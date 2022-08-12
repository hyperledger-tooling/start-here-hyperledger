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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    Allow maximum request timeout to be larger than write timeout (avoid EOF)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `WriteTimeout` in Go is actually the time all the way from the reading of the headers, until the data has been fully written in the response.

In an example E2E test with confirmations, so that synchronous calls take longer than 15s to complete, we see:

```
Websocket 127.0.0.1:5000 event: default/token_pool_confirmed/339d3f53-37de-4baa-bd46-e4277aeb315e -> c4a76e57-d586-4cbf-9581-b0deb5352ec4 (tx=%!s(*core.Transaction=<nil>))
    restclient.go:552: 
                Error Trace:    /Users/pbroadhurst/dev/firefly/firefly/test/e2e/runners/restclient.go:552
                                                        /Users/pbroadhurst/dev/firefly/firefly/test/e2e/runners/tokens.go:231
                Error:          Received unexpected error:
                                Post "http://127.0.0.1:5000/api/v1/namespaces/default/tokens/pools?confirm=true": EOF
                Test:           TestEthereumMultipartyE2ESuite/TestE2ENonFungibleTokensSync
```

This PR allows the constructor of the HTTP Server to include a MaximumRequestTimeout, which forces the read timeout and the write timeout (not the read header timeout) to be larger than this value.

It adds 1 second buffer, so that a nice error message can be returned in the case of a context based request timeout.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 20:22:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    Record defaults for array children
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently defaults are _not_ properly recorded if they are:
* set using `SetDefault` (rather than at creation time with `AddKnownKey`)
* a child or descendant of a config array

This PR fixes this functionality, along with bringing in the newest snapshot of Viper to pick up https://github.com/spf13/viper/pull/1387.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 20:02:56 +0000 UTC
    </div>
</div>

