---
layout: default
title: firefly-evmconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-evmconnect
---

# firefly-evmconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-evmconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Auto-backoff catchupPageSize if error matches configured regex pattern
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is intended to resolve FireFly issue https://github.com/hyperledger/firefly-evmconnect/pull/96.

The design is based on the assumption that different JSON/RPC providers will return slightly different errors for this scenario, so the event listener uses a (configurable) regex pattern when an error is returned from `eth_getLogs` to decide if it should be retried with a smaller `catchupPageSize`.

If `eth_getLogs` returns such an error, the page size is halved (the initial default being 500) until one of the following is true:

- the calls are successful
- the `catchupPageSize` reaches 1

(Reducing `catchupPageSize` to 1 is likely to mean the connector never catches up with main. It feels arbitrary to me however, to pick a higher value (10? 20?) that we set as a minimum to reduce the value down to so I've left the minimum as 1 for now.)

The value of `catchupPageSize` is only changed for the current runtime. This means that if the JSON/RPC endpoint is upgraded to support larger responses later then a restart of FireFly will return to the default catchupPageSize.

I haven't gone to the complexity of trying to slowly increase `catchupPageSize` back to a higher value, since this adds complexity for what feels like relatively little benefit. The most likely reason for a user hitting this is they are developer with a free JSON/RPC endpoint, not a production runtime. If they switch endpoint to a different one a restart is required anyway, so it feels like a suitable trade off.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 09:53:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    pick up fftm 1.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                picks up https://github.com/hyperledger/firefly-transaction-manager/pull/98
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-09 20:47:27 +0000 UTC
    </div>
</div>

