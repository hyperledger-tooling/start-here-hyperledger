---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1140" class=".btn">#1140</a>
            </td>
            <td>
                <b>
                    Update reqwest-client module documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the reqwest-client module documentation for stabilization.
This includes adding module level docs for the various `data` structs
and for the `ReqwestClient` struct itself.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 21:37:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1097" class=".btn">#1097</a>
            </td>
            <td>
                <b>
                    Stabilize client feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This stabilizes the `client` feature by moving it to `stable` from
`experimental`.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 21:46:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1082" class=".btn">#1082</a>
            </td>
            <td>
                <b>
                    Update references of "status" to "state"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the purchase order smart contract handler to use the
`workflow_state` field rather than `workflow_status`. This also updates
references of "status" to "state" to avoid confusion.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 20:03:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1081" class=".btn">#1081</a>
            </td>
            <td>
                <b>
                    Update purchase order man pages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the purchase order man pages to match the current implementation. This mainly included updating the formatting of arguments and updating the example responses.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 20:22:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1080" class=".btn">#1080</a>
            </td>
            <td>
                <b>
                    Add documentation comments for workflow module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds module-level and public API documentation for the
workflow module within the Grid SDK.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 19:19:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1079" class=".btn">#1079</a>
            </td>
            <td>
                <b>
                    Stabilize `rest-api-resources`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 19:04:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1078" class=".btn">#1078</a>
            </td>
            <td>
                <b>
                    Stabilize gridd "cylinder-jwt-support" by removing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change stabilizes the grid daemon's experimental
"cylinder-jwt-support" feature by removing it.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 16:16:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1077" class=".btn">#1077</a>
            </td>
            <td>
                <b>
                    Add Pike namespace to transaction inputs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds the Pike namespace to the Purchase Order smart
contract's transaction inputs. This allows the purchase order smart
contract to access the state within the Pike namespace.

Before this change, the sawtooth example would be unable to submit a purchase order smart contract action without receiving an error about attempting to access an unauthorized namespace (Pike Organization namespace, specifically).
```
sawtooth-sabre-tp                  | 2021-11-19 21:29:53,500 INFO  [sawtooth_sdk::processor] TP_PROCESS_REQUEST sending TpProcessResponse: ExternalsError { message: "Trap(Trap { kind: Host(ExternalsError { message: \"AuthorizationError(\\\"Tried to get unauthorized addresses: [\\\\\\\"621dee0501ba3ce58667ca9b12b3c0cdcc4da57f9962aeca7065c43a7d9c027332fdb9\\\\\\\"]\\\")\" }) })" }
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 15:32:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1076" class=".btn">#1076</a>
            </td>
            <td>
                <b>
                    Stabilize SDK's "cylinder-jwt-support" by removing it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change stabilizes the "cylinder-jwt-support" feature by removing it
from the Grid SDK.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 14:34:36 +0000 UTC
    </div>
</div>

