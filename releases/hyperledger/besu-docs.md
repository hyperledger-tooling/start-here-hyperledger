---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    24.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.7.0
                </span>
            </td>
            <td>
                ## 24.7.0

### Upcoming Breaking Changes
- Receipt compaction will be enabled by default in a future version of Besu. After this change it will not be possible to downgrade to the previous Besu version.
- PKI-backed QBFT will be removed in a future version of Besu. Other forms of QBFT will remain unchanged.
- --Xbonsai-limit-trie-logs-enabled is deprecated, use --bonsai-limit-trie-logs-enabled instead
- --Xbonsai-trie-logs-pruning-window-size is deprecated, use --bonsai-trie-logs-pruning-window-size instead
- `besu storage x-trie-log` subcommand is deprecated, use `besu storage trie-log` instead

### Breaking Changes
- `Xp2p-peer-lower-bound` has been removed. [#7247](https://github.com/hyperledger/besu/pull/7247)

### Additions and Improvements
- Support for eth_maxPriorityFeePerGas [#5658](https://github.com/hyperledger/besu/pull/7194)
- Improve genesis state performance at startup [#6977](https://github.com/hyperledger/besu/pull/6977)
- Enable continuous profiling with default setting [#7006](https://github.com/hyperledger/besu/pull/7006)
- A full and up to date implementation of EOF for Prague [#7169](https://github.com/hyperledger/besu/pull/7169)
- Add Subnet-Based Peer Permissions.  [#7168](https://github.com/hyperledger/besu/pull/7168)
- Reduce lock contention on transaction pool when building a block [#7180](https://github.com/hyperledger/besu/pull/7180)
- Update Docker base image to Ubuntu 24.04 [#7251](https://github.com/hyperledger/besu/pull/7251)
- Add LUKSO as predefined network name [#7223](https://github.com/hyperledger/besu/pull/7223)
- Refactored how code, initcode, and max stack size are configured in forks. [#7245](https://github.com/hyperledger/besu/pull/7245)
- Nodes in a permissioned chain maintain (and retry) connections to bootnodes [#7257](https://github.com/hyperledger/besu/pull/7257)
- Promote experimental `besu storage x-trie-log` subcommand to production-ready [#7278](https://github.com/hyperledger/besu/pull/7278)
- Enhanced BFT round-change diagnostics [#7271](https://github.com/hyperledger/besu/pull/7271)

### Bug fixes
- Validation errors ignored in accounts-allowlist and empty list [#7138](https://github.com/hyperledger/besu/issues/7138)
- Fix "Invalid block detected" for BFT chains using Bonsai DB [#7204](https://github.com/hyperledger/besu/pull/7204)
- Chain download halt fix(https://github.com/hyperledger/besu/pull/7162), fixes related issues: [#7109](https://github.com/hyperledger/besu/issues/7109)  [#6884](https://github.com/hyperledger/besu/issues/6884)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/24.7.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-05 16:49:57 +0000 UTC
    </span>
</div>

