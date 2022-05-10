---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3780" class=".btn">#3780</a>
            </td>
            <td>
                <b>
                    [MINOR] code cleanup - Lists.emptyList
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - changed some Longs to long where they were statically intialized
- changed random.nextLong() to random.nextInt(Integer.MAX_VALUE) to avoid the edge case of long minimum value which gives a negative value when passed into abs()
- replace deprecated Lists.emptyList() with Collections.emptyList()

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-03 11:58:43 +0000 UTC
    </div>
</div>

