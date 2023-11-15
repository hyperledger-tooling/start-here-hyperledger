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
                    23.10.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.10.2
                </span>
            </td>
            <td>
                ## Hyperledger Besu 23.10.2 
23.10.2 is an optional upgrade for Ethereum public and private networks. It is a **required update for Ethereum Classic Mordor network users** (not for ETC mainnet yet), as it contains the configuration for the Spiral network upgrade (#6078). It is recommended for Mainnet and private networks as there are several patches to vulnerable dependencies. 
### Upcoming Changes
- After we made the new layered TX pool default for all nodes in [23.10.0](https://github.com/hyperledger/besu/releases/tag/23.10.0), it caused some confusion and configuration issues among private network users. We know many of you are currently using the `legacy` pool, as it is better suited for larger nonce-gaps and gas free networks. This is a formal announcement of an upcoming naming change from this pool to better reflect its usage in private networks. This will have accompanying configuration changes as well, so stay tuned for the 23.4.0 release notes. Thank you for your patience as we update the two transaction pool implementations.  
### Breaking Changes
- TX pool eviction in the legacy TX pool now favours keeping oldest transactions (more likely to evict higher nonces, less likely to introduce nonce gaps) [#6106](https://github.com/hyperledger/besu/pull/6106) and [#6146](https://github.com/hyperledger/besu/pull/6146)
### Additions and Improvements
- Ethereum Classic Spiral upgrade for the Mordor network [#6078](https://github.com/hyperledger/besu/pull/6078)
- Add a method to read from a `Memory` instance without altering its inner state [#6073](https://github.com/hyperledger/besu/pull/6073)
- Accept `input` and `data` field for the payload of transaction-related RPC methods [#6094](https://github.com/hyperledger/besu/pull/6094)
- Add APIs to set and get the min gas price a transaction must pay for being selected during block creation [#6097](https://github.com/hyperledger/besu/pull/6097)
- TraceService: return results for transactions in block [#6087](https://github.com/hyperledger/besu/pull/6087)
- New option `--min-priority-fee` that sets the minimum priority fee a transaction must meet to be selected for a block. [#6080](https://github.com/hyperledger/besu/pull/6080) [#6083](https://github.com/hyperledger/besu/pull/6083)
- Implement new `miner_setMinPriorityFee` and `miner_getMinPriorityFee` RPC methods [#6080](https://github.com/hyperledger/besu/pull/6080)
- Clique config option `createemptyblocks` to not create empty blocks [#6082](https://github.com/hyperledger/besu/pull/6082)
- Upgrade EVM Reference Tests to v13 (Cancun) [#6114](https://github.com/hyperledger/besu/pull/6114)
- Add `yParity` to GraphQL and JSON-RPC for relevant querise. [6119](https://github.com/hyperledger/besu/pull/6119)
- Force tx replacement price bump to zero when zero base fee market is configured or `--min-gas-price` is set to 0. This allows for easier tx replacement in networks where there is not gas price. [#6079](https://github.com/hyperledger/besu/pull/6079)
- Introduce the possibility to limit the time spent selecting pending transactions during block creation, using the new experimental option `Xblock-txs-selection-max-time` on PoS and PoW networks (by default set to 5000ms) or `Xpoa-block-txs-selection-max-time` on PoA networks (by default 75% of the min block time) [#6044](https://github.com/hyperledger/besu/pull/6044)
- Remove LowestInvalidNonceCache from `legacy` transaction pool to make it more private networks friendly [#6148](https://github.com/hyperledger/besu/pull/6148)
### Bug fixes
- Upgrade netty to address CVE-2023-44487, CVE-2023-34462 [#6100](https://github.com/hyperledger/besu/pull/6100)
- Upgrade grpc to address CVE-2023-32731, CVE-2023-33953, CVE-2023-44487, CVE-2023-4785 [#6100](https://github.com/hyperledger/besu/pull/6100)
- Fix blob gas calculation in reference tests [#6107](https://github.com/hyperledger/besu/pull/6107)
- Limit memory used in handling invalid blocks [#6138](https://github.com/hyperledger/besu/pull/6138)

### Download Links 
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.10.2/besu-23.10.2.zip
597ab71898d379180106baf24878239ed49acefea5772344fd359b0ff13fe19f
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.10.2/besu-23.10.2.tar.gz
255818a5c6067a38aa8b565d8f32a49a172a7536a1d370673bbb75f548263c2c
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.10.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-11-15 15:24:32 +0000 UTC
    </span>
</div>

