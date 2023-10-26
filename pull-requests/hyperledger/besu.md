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
                PR <a href="https://github.com/hyperledger/besu/pull/6067" class=".btn">#6067</a>
            </td>
            <td>
                <b>
                    Don't put NONCE_TOO_LOW transactions into the invalid nonce cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This is intended to improve the issue described in https://github.com/hyperledger/besu/issues/6058. I don't think it fixes every possible case, but from testing it seems to be old transactions from a node, which are now all `NONCE_TOO_LOW`, that can cause this problem.

## Fixed Issue(s)
See https://github.com/hyperledger/besu/issues/6058 - although it may not be completely fixed after this PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-20 16:16:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6066" class=".btn">#6066</a>
            </td>
            <td>
                <b>
                    Update to production KZG ceremony output
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - update to new library
- disable KZG testing on static test vectors till new ones are available


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-20 14:29:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6064" class=".btn">#6064</a>
            </td>
            <td>
                <b>
                    Cherry-pick  main into release 23.10.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Cherry-pick main into release 23.10.x

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-20 01:51:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6062" class=".btn">#6062</a>
            </td>
            <td>
                <b>
                    Update changelog release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix changelog - Add issue numbers
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-20 00:24:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6060" class=".btn">#6060</a>
            </td>
            <td>
                <b>
                    Dencun corner cases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                cherry pick 2 changes from #6054 
* EIP-3541 regression in Cancun - https://github.com/hyperledger/besu/pull/6054/files#diff-22b78733e37a697fa8d1d8a02d2a87fe5ccea9cf67c34ce5e6311f024c14abd6L643-R738
* EIP-4788 conformance corner case - https://github.com/hyperledger/besu/pull/6054/files#diff-61db834b59eae5ce5c438462505de1add8fa244deda830742060d15f668a9806R39-R44
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 23:58:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6059" class=".btn">#6059</a>
            </td>
            <td>
                <b>
                    Trie log blobdb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->
## PR description
Move trie log storage to blobdb

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See #5866 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 22:59:29 +0000 UTC
    </div>
</div>

