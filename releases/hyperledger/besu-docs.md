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
                    22.7.0-RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.7.0-RC1
                </span>
            </td>
            <td>
                ### Additions and Improvements
- Do not require a minimum block height when downloading headers or blocks [#3911](https://github.com/hyperledger/besu/pull/3911)
- When on PoS the head can be only be updated by ForkchoiceUpdate [#3994](https://github.com/hyperledger/besu/pull/3994)
- Version information available in metrics [#3997](https://github.com/hyperledger/besu/pull/3997)
- Add TTD and DNS to Sepolia config [#4024](https://github.com/hyperledger/besu/pull/4024)
- Add terminal block hash and number to Ropsten genesis file [#4026](https://github.com/hyperledger/besu/pull/4026)
- Return `type` with value `0x0` when serializing legacy transactions [#4027](https://github.com/hyperledger/besu/pull/4027)
- Ignore `ForkchoiceUpdate` if `newHead` is an ancestor of the chain head [#4055](https://github.com/hyperledger/besu/pull/4055)

### Bug Fixes
- Fixed a snapsync issue that can sometimes block the healing step [#3920](https://github.com/hyperledger/besu/pull/3920)
- Support free gas networks in the London fee market [#4003](https://github.com/hyperledger/besu/pull/4003)
- Limit the size of outgoing eth subprotocol messages.  [#4034](https://github.com/hyperledger/besu/pull/4034)
- Fixed a state root mismatch issue on bonsai that may appear occasionally [#4041](https://github.com/hyperledger/besu/pull/4041)
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.7.0-RC1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-06-30 23:34:14 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.4.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.4.3
                </span>
            </td>
            <td>
                https://github.com/hyperledger/besu/releases/tag/22.4.3
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.4.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-06-30 23:34:14 +0000 UTC
    </span>
</div>

