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
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/40" class=".btn">#40</a>
            </td>
            <td>
                <b>
                    fix leaf deletion issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->

## PR description

This PR fixes a bug that occurs when removing a key from a trie that isn't loaded. In a certain configuration, when we want to check if an internal node has only one child, we verify how many children are not NullNodes. However, when the node is not loaded, they are not NullNodes but StoredNodes. So, in the current code, we need to load the StoredNodes to see if they are null or not.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 14:50:47 +0000 UTC
    </div>
</div>

