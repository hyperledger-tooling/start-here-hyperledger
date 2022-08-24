---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/974" class=".btn">#974</a>
            </td>
            <td>
                <b>
                    Leverage transaction cache in a few more places
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-17 18:33:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/973" class=".btn">#973</a>
            </td>
            <td>
                <b>
                    fix integration matrix `exclude`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `exclude` was not correctly handling arrays, so it has been updated to explicitly define all excluded combinations

list of jobs that will be executed now (courtesy of [act](https://github.com/nektos/act)):


-  `[blockchain-provider:besu database-type:postgres test-suite:TestEthereumMultipartyE2ESuite]`
- `[blockchain-provider:geth database-type:sqlite3 test-suite:TestEthereumMultipartyE2ESuite]`
- `[blockchain-provider:geth database-type:postgres test-suite:TestEthereumMultipartyE2ESuite]`
- `[blockchain-provider:geth database-type:sqlite3 test-suite:TestEthereumGatewayE2ESuite]`
- `[blockchain-provider:geth database-type:postgres test-suite:TestEthereumGatewayE2ESuite]`
- `[blockchain-provider:besu database-type:sqlite3 test-suite:TestEthereumGatewayE2ESuite]`
- `[blockchain-provider:besu database-type:postgres test-suite:TestEthereumGatewayE2ESuite]`
- `[bockchain-provider:geth database-type:sqlite3 test-suite:TestEthereumMultipartyTokensRemoteNameE2ESuite]`
- `[blockchain-provider:geth database-type:postgres test-suite:TestEthereumMultipartyTokensRemoteNameE2ESuite]`
- `[blockchain-provider:besu database-type:sqlite3 test-suite:TestEthereumMultipartyTokensRemoteNameE2ESuite]`
- `[blockchain-provider:besu database-type:postgres test-suite:TestEthereumMultipartyTokensRemoteNameE2ESuite]`
- `[blockchain-provider:fabric database-type:sqlite3 test-suite:TestFabricGatewayE2ESuite]`
- `[blockchain-provider:fabric database-type:postgres test-suite:TestFabricGatewayE2ESuite]`
- `[blockchain-provider:fabric database-type:sqlite3 test-suite:TestFabricMultipartyE2ESuite]`
- `[blockchain-provider:fabric database-type:postgres test-suite:TestFabricMultipartyE2ESuite]`

closes #968 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-17 18:04:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/972" class=".btn">#972</a>
            </td>
            <td>
                <b>
                    Add cache for operations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-17 17:04:19 +0000 UTC
    </div>
</div>

