---
layout: default
title: besu-verkle-trie
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-verkle-trie
---

# besu-verkle-trie <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-verkle-trie){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    fix main storage offset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->

## PR description

should be UInt256.valueOf(256).pow(31) , but there is currently a bug in the testnet and instead, the other clients are using a shift left operation. So we are doing a shift left to follow the testnet, but this should be fixed later.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 14:39:43 +0000 UTC
    </div>
</div>

