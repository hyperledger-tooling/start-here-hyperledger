---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    [wsclient] Allow for Embedded Basic Auth in URLs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We observed when using the `wsclient` package that if a WS URL had basic auth embedded in it we'd get the following error:
```
Kaleido Block IndexerCopyright (C) 2023 Kaleido
Version:  (Build Date: 2023-11-16T19:49:14Z)

time="2023-11-20T20:14:29.999Z" level=info msg="[i] No TLS configuration provided`"
time="2023-11-20T20:14:29.999Z" level=debug msg="Created REST client to https://user:pass@acme.com"
time="2023-11-20T20:14:29.999Z" level=warning msg="WS wss://user:pass@acme.com connect attempt 1 failed [-1]: "
time="2023-11-20T20:14:29.999Z" level=fatal msg="[!] Failed to connect to blockchain : FF00148: Websocket connect failed: malformed ws or wss URL"
```

In some cases, applied configurations are more difficult to change than a binary version. This change proposes that the credentials in the URL be handled more gracefully, in that 1) the embedded credentials are always removed from the URL string, and that 2) if the config did not have auth credentials provided, the embedded credentials are extracted and used automatically.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 05:41:07 +0000 UTC
    </div>
</div>

