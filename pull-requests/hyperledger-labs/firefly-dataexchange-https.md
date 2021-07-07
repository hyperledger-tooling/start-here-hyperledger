---
layout: default
title: firefly-dataexchange-https
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-dataexchange-https
---

# firefly-dataexchange-https <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-dataexchange-https){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    Decoupling Peers from config.json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While working on https://github.com/hyperledger-labs/firefly/pull/114, I understood `config.json` needs to be writeable solely for the sake of the `peers`. To me this indicated a difference between config (provided at start time and only changeable on restart) vs data (dynamic during runtime, does not require restart). Talking w/ @gabriel-indik confirmed this was a result of how DX has evolved over time.

While we could have it so that DX has init containers to copy over an initial config provided from a `Secret` to a writeable location, we get into challenges around detecting if config like `apiKey` or `p2p.endpoint` changes and having to reconcile the K8s/cloud provided config w/ the live, writeable config.

It felt easier to do some of the work now, and make `peers` a separate, writeable JSON file and have the two pieces of data get merged at load time. Additionally, if the `peers/data.json` does not exist it just sets the peers list to empty to avoid additional bootstrapping (though the subdirectory does have to be made...).

I'm wondering if `config.json`, `key.pem`, `cert.pem`, and `ca.pem` shouldn't be in an entirely separate separate folder i.e. /config so that the two directories can be have different permissions i.e. readable vs writeable. Looking for feedback there as opposed to having peers/data.json be a subfolder.

Also includes a bug related to reading CAs from EBS-backed PVCs, see https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/28#issuecomment-875219742
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 15:58:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/27" class=".btn">#27</a>
            </td>
            <td>
                <b>
                    Graceful Shutdown for Cloud-Native Environments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While running DX on K8s as part of https://github.com/hyperledger-labs/firefly/pull/114 I noticed pods would take the entire grace period before properly shutting down. Handling `INT` and `QUIT` will make it so we properly shut down when K8s terminates a pod (rather than using a CLI tool like `dumb-init`):

Output from testing:

First terminal where I ran DX
```shell
❯ npm start

> firefly-dataexchange@1.0.0 start
> node build/index.js

2021-07-02T15:22:32.819Z [INFO ]: FireFly Data Exchange running on http://0.0.0.0:3000 (API) and https://0.0.0.0:3001 (P2P) - log level "info" app.ts
2021-07-02T15:22:52.525Z [INFO ]: FireFly Data Exchange is gracefully shutting down app.ts
❯ npm start

> firefly-dataexchange@1.0.0 start
> node build/index.js

2021-07-02T15:22:59.358Z [INFO ]: FireFly Data Exchange running on http://0.0.0.0:3000 (API) and https://0.0.0.0:3001 (P2P) - log level "info" app.ts
2021-07-02T15:23:10.018Z [INFO ]: FireFly Data Exchange is gracefully shutting down app.ts
❯ npm start

> firefly-dataexchange@1.0.0 start
> node build/index.js

2021-07-02T15:23:17.321Z [INFO ]: FireFly Data Exchange running on http://0.0.0.0:3000 (API) and https://0.0.0.0:3001 (P2P) - log level "info" app.ts
2021-07-02T15:23:35.168Z [INFO ]: FireFly Data Exchange is gracefully shutting down app.ts
```

And terminal where I killed DX:
```
❯ ps aux | grep node
hfuss            16607   0.0  0.3  4767956  55500 s002  S+   11:22AM   0:00.61 node build/index.js
❯ kill -s QUIT 16607
❯ ps aux | grep node
hfuss            16612   0.0  0.3  4730180  57820 s002  S+   11:22AM   0:00.51 node build/index.js
❯ kill -s QUIT 16612
❯ ps aux | grep node
hfuss            16616   0.1  0.3  4785220  57936 s002  S+   11:23AM   0:00.57 node build/index.js
❯ kill -s TERM 16616
```

Will defer to @gabriel-indik @peterbroadhurst if any additional shutdown logic should be added to `stop` i.e. wait for all in-flight HTTP requests to finish, writing to disk operations, etc.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 15:29:49 +0000 UTC
    </div>
</div>

