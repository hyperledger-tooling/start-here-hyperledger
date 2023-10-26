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
                    23.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.10.1
                </span>
            </td>
            <td>
                ## 23.10.1

### Additions and Improvements
- New option `--tx-pool-priority-senders` to specify a list of senders, that has the effect to prioritize any transactions sent by these senders from any source [#5959](https://github.com/hyperledger/besu/pull/5959)
- Cache last n blocks by using a new Besu flag `--cache-last-blocks=n` [#6009](https://github.com/hyperledger/besu/pull/6009)
- Optimize performances of RPC method `eth_feeHistory` [#6011](https://github.com/hyperledger/besu/pull/6011) #6035
- Logging summary of plugins at Info as part of the config overview #5964 #6049
- Layered tx pool memory improvements #5985 #5974 
- Update Bouncy Castle to 1.76, and force the use of the `jdk18on` variant #5748 
- Add GraphQL support for new fields in Cancun [#5923](https://github.com/hyperledger/besu/pull/5930) #5975
- Add new configuration options to the EVM Fluent APIs [#5930](https://github.com/hyperledger/besu/pull/5930)


### Deprecations
- `--tx-pool-disable-locals` has been deprecated for removal in favor of `--tx-pool-no-local-priority`, no semantic change, only a renaming [#5959](https://github.com/hyperledger/besu/pull/5959)

### Bug Fixes
- Fix regression with t8n tool filling #5979
- Fix EOF and EIP-4788 regressions in reference tests #6060

### Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.10.1/besu-23.10.1.tar.gz / sha256: e27645f345583f3ee447e5418302382c6f8335d2da8707bdd20033aabd86ce4c

https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.10.1/besu-23.10.1.zip / sha256: fb173acb93c72fbb74a6542051691ca2d3d5f54ea2f51026467a512f3a22106b
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.10.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-10-25 02:24:27 +0000 UTC
    </span>
</div>

