---
layout: default
title: yui-docs
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-docs
---

# yui-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-docs/pull/77" class=".btn">#77</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/crypto from 0.9.0 to 0.17.0 in /samples/minitoken-besu-ethereum/relayer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/crypto](https://github.com/golang/crypto) from 0.9.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/crypto/commit/9d2ee975ef9fe627bf0a6f01c1f69e8ef1d4f05d"><code>9d2ee97</code></a> ssh: implement strict KEX protocol changes</li>
<li><a href="https://github.com/golang/crypto/commit/4e5a26183ecb4f9a0f85c8f8dbe7982885435436"><code>4e5a261</code></a> ssh: close net.Conn on all NewServerConn errors</li>
<li><a href="https://github.com/golang/crypto/commit/152cdb1503ebc13bc0fbb68f92ee189ebf9e3d00"><code>152cdb1</code></a> x509roots/fallback: update bundle</li>
<li><a href="https://github.com/golang/crypto/commit/fdfe1f8531a1adcc300c8eba98cb372044826d62"><code>fdfe1f8</code></a> ssh: defer channel window adjustment</li>
<li><a href="https://github.com/golang/crypto/commit/b8ffc16e10063067bac0e15c6d7f7995937503ce"><code>b8ffc16</code></a> blake2b: drop Go 1.6, Go 1.8 compatibility</li>
<li><a href="https://github.com/golang/crypto/commit/7e6fbd82c804e1760feb603fe21caecb0af0a124"><code>7e6fbd8</code></a> ssh: wrap errors from client handshake</li>
<li><a href="https://github.com/golang/crypto/commit/bda2f3f5cfce3f27039acccd823693f6d67c2a74"><code>bda2f3f</code></a> argon2: avoid clobbering BP</li>
<li><a href="https://github.com/golang/crypto/commit/325b735346247f48971d2b37d24dd180a35f391f"><code>325b735</code></a> ssh/test: skip TestSSHCLIAuth on Windows</li>
<li><a href="https://github.com/golang/crypto/commit/1eadac50a566dfaa1b603ca15e8ad3cbd1c77b20"><code>1eadac5</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/crypto/commit/b2d7c26edb17864f117d8b0ee73c1843bcc6090f"><code>b2d7c26</code></a> ssh: add (*Client).DialContext method</li>
<li>Additional commits viewable in <a href="https://github.com/golang/crypto/compare/v0.9.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/crypto&package-manager=go_modules&previous-version=0.9.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/yui-docs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 00:21:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-docs/pull/76" class=".btn">#76</a>
            </td>
            <td>
                <b>
                    Increase sleep duration in Makefile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I followed the instructions in the `samples/minitoken-besu-ethereum` and ran `make setup`, but I encountered the following error. 
By ensuring sufficient sleep time after starting the Blockchain node, I resolved this error. I think this is dependent on the local environment, but there's a possibility that 5 seconds may not be enough.

- My local environment: [MacBook Air (15 inch, M2, 2023)](https://support.apple.com/kb/SP893)

```
$ make setup       
npm run compile

> minitoken@1.0.0 compile
> truffle compile


Compiling your contracts...
===========================
> Everything is up to date, there is nothing to compile.
go build -o ../build/uly .
docker compose build --no-cache
[+] Building 17.6s (22/22) FINISHED                                                                                                                                                                      
 => [ibc1 internal] load build definition from Dockerfile                                                                                                                                           0.0s
 => => transferring dockerfile: 491B                                                                                                                                                                0.0s
 => [ibc1 internal] load .dockerignore                                                                                                                                                              0.0s
 => => transferring context: 2B                                                                                                                                                                     0.0s
 => [ibc0 internal] load build definition from Dockerfile                                                                                                                                           0.0s
 => => transferring dockerfile: 651B                                                                                                                                                                0.0s
 => [ibc0 internal] load .dockerignore                                                                                                                                                              0.0s
 => => transferring context: 2B                                                                                                                                                                     0.0s
 => [ibc1 internal] load metadata for docker.io/ethereum/client-go:v1.11.6                                                                                                                          2.7s
 => [ibc0 internal] load metadata for docker.io/hyperledger/besu:21.1                                                                                                                               2.7s
 => CACHED [ibc1 1/7] FROM docker.io/ethereum/client-go:v1.11.6@sha256:5d7f40c92c152d7a7da6f1570da468b21d5cb728e91ad281749bf213a1d4a892                                                             0.0s
 => [ibc1 internal] load build context                                                                                                                                                              0.0s
 => => transferring context: 270B                                                                                                                                                                   0.0s
 => CACHED [ibc0 1/6] FROM docker.io/hyperledger/besu:21.1@sha256:0c548b0bd410252129785bacf544f215f1efd7b736c835eaef92fdeef42bafa5                                                                  0.0s
 => => resolve docker.io/hyperledger/besu:21.1@sha256:0c548b0bd410252129785bacf544f215f1efd7b736c835eaef92fdeef42bafa5                                                                              0.0s
 => [ibc0 internal] load build context                                                                                                                                                              0.0s
 => => transferring context: 78B                                                                                                                                                                    0.0s
 => [ibc0 2/6] RUN mkdir -p /tmp/besu/data                                                                                                                                                          0.4s
 => [ibc1 2/7] ADD geth.password /root/geth.password                                                                                                                                                0.0s
 => [ibc1 3/7] ADD genesis.json  /root/genesis.json                                                                                                                                                 0.0s
 => [ibc1 4/7] ADD privatekey  /root/privatekey                                                                                                                                                     0.0s
 => [ibc1 5/7] ADD run.sh  /run.sh                                                                                                                                                                  0.0s
 => [ibc1 6/7] RUN /usr/local/bin/geth --nousb --datadir /root/.ethereum init /root/genesis.json                                                                                                    0.9s
 => [ibc0 3/6] WORKDIR /tmp/besu                                                                                                                                                                    0.0s
 => [ibc0 4/6] ADD ibftConfigFile.json /tmp/besu/ibftConfigFile.json                                                                                                                                0.0s
 => [ibc0 5/6] RUN besu operator generate-blockchain-config --config-file=ibftConfigFile.json --to=networkFiles --private-key-file-name=key                                                        13.9s
 => [ibc1 7/7] RUN /usr/local/bin/geth --nousb account import --password /root/geth.password /root/privatekey                                                                                       8.8s
 => [ibc0] exporting to image                                                                                                                                                                       0.1s
 => => exporting layers                                                                                                                                                                             0.0s
 => => writing image sha256:ec3f036e1648c22123b928b7d4b7ce4d515b0f0d8045ac2ed3b9fc9dd77e938a                                                                                                        0.0s
 => => naming to docker.io/library/chains-ibc1                                                                                                                                                      0.0s
 => => writing image sha256:05361967e06f82162c54c1f117e285bb0b9431df7fde0a9fb8f10d953354730f                                                                                                        0.0s
 => => naming to docker.io/library/chains-ibc0                                                                                                                                                      0.0s
 => [ibc0 6/6] RUN cp ./networkFiles/keys/*/* ./data/                                                                                                                                               0.4s
docker compose up -d
[+] Running 3/3
 ✔ Network chains_default   Created                                                                                                                                                                 0.1s 
 ✔ Container chains-ibc1-1  Started                                                                                                                                                                 0.5s 
 ✔ Container chains-ibc0-1  Started                                                                                                                                                                 0.5s 
sleep 5
npm run migrate:ibc0

> minitoken-besu-ethereum@1.0.0 migrate:ibc0
> truffle migrate --network=ibc0 --compile-none


Compiling your contracts...
===========================
> Compilation skipped because --compile-none option was passed.

/Users/mattsu6666/ghq/github.com/hyperledger-labs/yui-docs/samples/minitoken-besu-ethereum/node_modules/eth-block-tracker/src/polling.js:51
        const newErr = new Error(`PollingBlockTracker - encountered an error while attempting to update latest block:\n${err.stack}`)
                       ^
Error: PollingBlockTracker - encountered an error while attempting to update latest block:
undefined
    at PollingBlockTracker._performSync (/Users/mattsu6666/ghq/github.com/hyperledger-labs/yui-docs/samples/minitoken-besu-ethereum/node_modules/eth-block-tracker/src/polling.js:51:24)
    at processTicksAndRejections (node:internal/process/task_queues:95:5)
UnhandledRejections detected
Promise {
  <rejected> {
    code: -32603,
    message: 'socket hang up',
    data: { originalError: [Object] }
  }
} {
  code: -32603,
  message: 'socket hang up',
  data: { originalError: { code: 'ECONNRESET' } }
}
make: *** [migrate] Error 1
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 05:05:50 +0000 UTC
    </div>
</div>

