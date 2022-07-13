---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/225" class=".btn">#225</a>
            </td>
            <td>
                <b>
                    Update to Go 1.17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update build to go 1.17 consistent with other FireFly repos.

Also updates the bundled solidity compiler version in the default docker build in this repo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 12:15:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/224" class=".btn">#224</a>
            </td>
            <td>
                <b>
                    Do not require the filter id to be numeric
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The JSON/RPC spec has previously stated that the result of an `eth_newFitler` will be a `QUANTITY`, and that is so in Besu/Go-ethereum (and derivatives). However, we've found that there are EVM chain node implementations return other values, such as a UUID encoded to a string.

EthConnect doesn't have any reason to rely on it being a numeric, as it's just an opaque value that stores and sends back on future calls.

The latest generated official docs (at the current point less detailed than the previous wiki based docs) Ethereum JSON/RPC spec docs state `string` as the result:
https://ethereum.github.io/execution-apis/api-documentation/

So this PR moves EthConnect to just use a string
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 11:30:30 +0000 UTC
    </div>
</div>

