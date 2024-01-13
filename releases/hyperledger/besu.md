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
                    24.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.1.0
                </span>
            </td>
            <td>
                ## 24.1.0 Quarterly
This release is a strongly recommended update for all Mainnet users. **24.1.0 is a required release for the upcoming Ethereum testnet forks**, the first of which is Goerli on the 17th of January.  **This is also a required update for all ETC node operators as it contains the configurations for the Spiral hard fork.** 24.1.0 contains some optional, but useful features for private networks.

This release includes the latest hotfix for the Mainnet halt Besu experienced on January 6th. A post-mortem of that bug can be found [here](https://wiki.hyperledger.org/pages/viewpage.action?pageId=117440824). This release contains many related Bonsai fixes. 

### Deprecations
- Forest pruning (`pruning-enabled` options) is deprecated and will be removed soon. To save disk space consider switching to Bonsai data storage format [#6230](https://github.com/hyperledger/besu/pull/6230)

### Additions and Improvements
- Add error messages on authentication failures with username and password [#6212](https://github.com/hyperledger/besu/pull/6212)
- New `Sequenced` transaction pool. The pool is an evolution of the `legacy` pool and is likely to be more suitable to enterprise or permissioned chains than the `layered` transaction pool. Select to use this pool with `--tx-pool=sequenced`. Supports the same options as the `legacy` pool [#6274](https://github.com/hyperledger/besu/issues/6274)
- Set Ethereum Classic mainnet activation block for Spiral network upgrade [#6267](https://github.com/hyperledger/besu/pull/6267)
- Add custom genesis file name to config overview if specified [#6297](https://github.com/hyperledger/besu/pull/6297)
- Update Gradle plugins and replace unmaintained License Gradle Plugin with the actively maintained Gradle License Report [#6275](https://github.com/hyperledger/besu/pull/6275)
- Cancun forkids for non-mainnets [#6322](https://github.com/hyperledger/besu/pull/6322)

### Bug fixes
- Hotfix for selfdestruct preimages on bonsai #6359 
- Fix trielog shipping issue during self destruct #6340
- Mitigation for trielog failure #6315

### Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/24.1.0/besu-24.1.0.zip / sha256 d36c8aeef70f0a516d4c26d3bc696c3e2a671e515c9e6e9475a31fe759e39f64
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/24.1.0/besu-24.1.0.tar.gz / sha256 602b04c0729a7b17361d1f0b39f4ce6a2ebe47932165add666560fe594d9ca99 
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.1.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-01-08 22:01:19 +0000 UTC
    </span>
</div>

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

