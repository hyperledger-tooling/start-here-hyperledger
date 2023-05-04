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
                    23.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.4.0
                </span>
            </td>
            <td>
                This quarterly update should be carefully reviewed by private network users before upgrading. This quarterly release contains a lot of new improvements but many breaking changes. We have deprecated GoQuorum-compatible privacy modes in this release, as well as IBFT1.0. If you require these, please consider migrating to new consensus algorithms or waiting for future releases.

Highlights in this release include:

- RocksDB 8 upgrade that improves the performance of the underlying database.
- Many logging and metrics improvements across the client.
- EVM performance improvements.
- An improved gas estimation algorithm.
- Fixes for QBFT and IBFT using zeroBaseFee
- RPC fixes
- Many more.

Lastly, this release formalizes a deprecation notice for GoQuorum -compatible permissioning modes in Besu. These will be removed in the 23.7 series, unless otherwise stated.
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/23.4.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-05-02 17:55:16 +0000 UTC
    </span>
</div>

