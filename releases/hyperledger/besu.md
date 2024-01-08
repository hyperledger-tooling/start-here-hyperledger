---
layout: default
title: besu
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    23.10.3-hotfix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.10.3-hotfix
                </span>
            </td>
            <td>
                ## 23.10.3-hotfix
This is a hotfix for a selfdestruct defect that occurred on mainnet at block [18947893](https://etherscan.io/block/18947893)

- Hotfix for selfdestruct preimages on bonsai [#6359]((https://github.com/hyperledger/besu/pull/6359)
- mitigation for trielog failure [#6315]((https://github.com/hyperledger/besu/pull/6315)


This release fixes the root of the problem, but Besu needs to be resynced in order to repair the state.  The fastest way to do this is to trigger a backward sync in Besu. After installing the hotfix, your CL client will need to have its beacon state reset and restored using checkpoint sync. Recovering from a deleted beacon chain is much faster if you have Checkpoint Sync setup, which is CL client specific.

Instructions on how to delete the beacon db, depends on your client.  For example for Teku, you need to remove the beacon folder in the Teku data path. For other clients, refer to their documentation. 

Most users should be good to go. If this doesn't work, please try the below instructions and report your problem to the Hyperledger Discord at https://discord.gg/hyperledger

Try the same process again, but force Besu to set its head back to a block prior to the problem block. This will require API access, and for this to work you have to enabled the DEBUG API with the following startup options:

` --rpc-http-api=ETH,NET,WEB3,DEBUG `

See [RPC APIs](https://besu.hyperledger.org/public-networks/reference/cli/options#rpc-http-api) for more details, changes to that param will require Besu to be restarted.

Once Besu is up and you have access to `DEBUG` apis, you can shutdown your CL client and clear its database. With Besu still up, set its head back to block 18947892 (0x1211F34 in hex) using the following API call:

`curl -X POST --data '{"jsonrpc":"2.0","method":"debug_setHead","params":["0x1211F34"],"id":1}' http://localhost:8545`

Then restart your CL. Your CL should optimistically sync the beacon chain using a checkpoint from the network, and this will trigger a backward sync in Besu. 


If your client still isn't progressing, you can try to resync only the world state.  It can take hours, but it is faster from a resync from scratch

`curl -X POST --data '{"jsonrpc":"2.0","method":"debug_resyncWorldState","params":[],"id":1}' http://localhost:8545`


### Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.10.3-hotfix/besu-23.10.3-hotfix.zip / sha256 1c37762909858a40eca749fb85b77fb4d1e918f247aff56d518144828bd85378
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.10.3-hotfix/besu-23.10.3-hotfix.tar.gz / sha256 8e38e9fd0c16e049aa324effc96f9ec31dc06e82ea4995e9dd75d571394667af

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.10.3-hotfix" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-01-06 23:59:59 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    23.10.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.10.3
                </span>
            </td>
            <td>
                ## 23.10.3

### Additions and Improvements
- Implement debug_traceCall [#5885](https://github.com/hyperledger/besu/pull/5885)
- Transactions that takes too long to evaluate, during block creation, are dropped from the txpool [#6163](https://github.com/hyperledger/besu/pull/6163)
- New option `tx-pool-min-gas-price` to set a lower bound when accepting txs to the pool [#6098](https://github.com/hyperledger/besu/pull/6098)
- Update OpenJDK latest Docker image to use Java 21 [#6189](https://github.com/hyperledger/besu/pull/6189)
- Allow a transaction selection plugin to specify custom selection results [#6190](https://github.com/hyperledger/besu/pull/6190)
- Add `rpc-gas-cap` to allow users to set gas limit to the RPC methods used to simulate transactions[#6156](https://github.com/hyperledger/besu/pull/6156)
- Fix the unavailability of `address` field when returning an `Account` entity on GraphQL in case of unreachable world state [#6198](https://github.com/hyperledger/besu/pull/6198)
- Update OpenJ9 Docker image to latest version [#6226](https://github.com/hyperledger/besu/pull/6226)
- Add error messages on authentication failures with username and password [#6212](https://github.com/hyperledger/besu/pull/6212)
- Add `rocksdb usage` to the `storage` subcommand to allow users and dev to check columns families usage [#6185](https://github.com/hyperledger/besu/pull/6185)
- Ethereum Classic Spiral network upgrade [#6078](https://github.com/hyperledger/besu/pull/6078)

### Bug fixes
- Fix Docker image name clash between Besu and evmtool [#6194](https://github.com/hyperledger/besu/pull/6194)
- Fix `logIndex` in `eth_getTransactionReceipt` JSON RPC method [#6206](https://github.com/hyperledger/besu/pull/6206)

### Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.10.3/besu-23.10.3.zip / sha256 da7ef8a6ceb88d3e327cacddcdb32218d1750b464c14165a74068f6dc6e0871a
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.10.3/besu-23.10.3.tar.gz / sha256 73c834cf32c7bbe255d7d8cc7ca5d1eb0df8430b9114935c8dcf3a675b2acbc2

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.10.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-12-30 20:21:13 +0000 UTC
    </span>
</div>

