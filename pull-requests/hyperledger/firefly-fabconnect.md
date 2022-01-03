---
layout: default
title: firefly-fabconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-fabconnect
---

# firefly-fabconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-fabconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/69" class=".btn">#69</a>
            </td>
            <td>
                <b>
                    Fixed runtime path for spec.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jim Zhang <jim.zhang@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-03 18:05:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/68" class=".btn">#68</a>
            </td>
            <td>
                <b>
                    Add spec.yaml to runtime image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Missed this when adding the API spec capability. The static resource must be added to the runtime image for it to be available to serve to present the Swagger UI
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-03 16:57:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/67" class=".btn">#67</a>
            </td>
            <td>
                <b>
                    Add transaction index to the event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This helps with sequencing on the client side when there are multiple events fired in the same block
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-30 02:24:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fabconnect/pull/65" class=".btn">#65</a>
            </td>
            <td>
                <b>
                    API spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - serves the Swagger UI on `/api` endpoint with the openapi 3.0 yaml
- enhanced the transaction receipt with information that got lost previously (block number, tx id, etc.)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 23:13:07 +0000 UTC
    </div>
</div>

