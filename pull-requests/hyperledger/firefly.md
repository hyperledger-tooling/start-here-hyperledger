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
                PR <a href="https://github.com/hyperledger/firefly/pull/995" class=".btn">#995</a>
            </td>
            <td>
                <b>
                    Update ERC-1155 connector and evmconnect for RC.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-20 04:06:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/994" class=".btn">#994</a>
            </td>
            <td>
                <b>
                    Wait for server to exit, before restarting for reset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/firefly/issues/993

We need to wait for the `startFirefly` routine to exit, before we can safely restart it.

This means a second channel to distinguish exit, from an error.

A secondary fix in this PR, is to stop/restart the debug server after the reset - previously it was never stopped.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-20 03:51:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/992" class=".btn">#992</a>
            </td>
            <td>
                <b>
                    Propagate the underlying parse error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Found while diagnosing https://github.com/hyperledger/firefly/issues/990#issuecomment-1221077085, that we didn't include the underlying error when we had a problem parsing the input for the Ethereum implementation of the `/api/v1/contracts/interfaces/generate` endpoint.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-19 20:46:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/991" class=".btn">#991</a>
            </td>
            <td>
                <b>
                    Add /pins/rewind API for requesing manual rewind
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Mitigation for https://github.com/hyperledger/firefly/issues/986 and similar issues.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-19 19:27:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/988" class=".btn">#988</a>
            </td>
            <td>
                <b>
                    Restore camelCase key names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since the Viper patch has been absorbed (#930), it's OK to use
camelCase in config files again.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-19 14:55:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/987" class=".btn">#987</a>
            </td>
            <td>
                <b>
                    Update firefly_node.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Typo fix PostgreSQL.

Signed-off-by: Liad Cohen <6436094+Liadc@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 23:03:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/984" class=".btn">#984</a>
            </td>
            <td>
                <b>
                    Fix bugs when running with an old config file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                FireFly should continue to work when run against a config file from 1.0.x.

Since this references 1.0.4, it should go in after https://github.com/hyperledger/firefly/pull/982 is merged and released as 1.0.4.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 19:38:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/983" class=".btn">#983</a>
            </td>
            <td>
                <b>
                    bump reset polling to 60seconds
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
        Created At 2022-08-18 18:31:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/982" class=".btn">#982</a>
            </td>
            <td>
                <b>
                    Misc cleanup for 1.0 branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Explicitly log the deprecation of the "publicstorage" key
* Update the CLI to 1.0.2
* Backport ffconfig tool
* Pin golangci-lint to an older version
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 17:43:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/981" class=".btn">#981</a>
            </td>
            <td>
                <b>
                    add nil check for aggregator during WaitStop
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
        Created At 2022-08-18 17:08:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/980" class=".btn">#980</a>
            </td>
            <td>
                <b>
                    Add nil check for blobReceiver during WaitStop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #979
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 16:01:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/977" class=".btn">#977</a>
            </td>
            <td>
                <b>
                    Use optimistic inserts for blockchain events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Always attempt to insert first, then fall back to a query for duplicates.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 15:01:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/976" class=".btn">#976</a>
            </td>
            <td>
                <b>
                    Only query operations from the database if there were cache misses
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
        Created At 2022-08-17 22:13:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/975" class=".btn">#975</a>
            </td>
            <td>
                <b>
                    Adjust defaults for all cache items that don't expose a Size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                Caches may be limited on size (if the items advertise their Size) or on
number of items. Since most cached items do not expose a Size, the limit
should be set on number of items alone.

Picked numbers pretty much at random, so I'm open to feedback if they
should be higher or lower, or if any of these items should get a Size method
to do size estimation.

I've tagged with "migration_consideration" since I have renamed a few
config keys, but I don't think they're widely used.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-17 19:48:15 +0000 UTC
    </div>
</div>

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/971" class=".btn">#971</a>
            </td>
            <td>
                <b>
                    Fix group race condition, optimize transaction cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Insert local group only after inserting groupinit message.
This ensures no other threads pick up on the group before the
message is sequenced.

Update transaction cache after initial insert.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 17:53:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/970" class=".btn">#970</a>
            </td>
            <td>
                <b>
                    Update to firefly-signer v0.9.15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 15:51:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/969" class=".btn">#969</a>
            </td>
            <td>
                <b>
                    Update to firefly-signer v0.9.13
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 15:07:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/967" class=".btn">#967</a>
            </td>
            <td>
                <b>
                    Performance improvements for batch lookups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure batch ID queries match the current indexes (to avoid sequential scan), and improve the caching in aggregator when processing a group of pins.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 04:15:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/966" class=".btn">#966</a>
            </td>
            <td>
                <b>
                    Add tutorial for Polygon testnet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rendered preview is currently available at: https://nguyer.github.io/firefly/head/tutorials/chains/polygon_testnet.html
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 20:59:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/965" class=".btn">#965</a>
            </td>
            <td>
                <b>
                    bump ui to 1.1 alpha 3
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
        Created At 2022-08-15 19:41:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/963" class=".btn">#963</a>
            </td>
            <td>
                <b>
                    Update to latest dependencies ready for V1.1 alpha.3
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
        Created At 2022-08-15 16:42:59 +0000 UTC
    </div>
</div>

