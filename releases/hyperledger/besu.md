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

