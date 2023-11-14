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
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Fix IPA description in javadocs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix IPA description
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-13 20:36:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    FIX: bugs in visitors and nodes to make testDeleteManyValues pass
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

testDeleteManyValuesWithDivergentStemsAtDepth2 was added from previous besu Merkle tests. The test allowed to detect several bugs in visitors and nodes, that were all fixed. Javadoc was also made to emit no warnings.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-11 17:11:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Fix javadoc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->

## PR description

Fix javadoc issues for pipeline 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-10 09:22:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    REFACTOR: Addition of StemNodes to capture SuffixExtensions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This is a major refactoring that solves several problems:

  - Ready to generate proof data: StemNodes capture the suffix-extensions from the specs, with its intermediate commitments.
  - Root hashes can be tested against testnet: they are coherent with go-verkle and rust-verkle.
  - Trie can be stored/retrieved from database: StoredVerkleTrie makes it transparent to work with a Trie that is not completely loaded in memory and looks for nodes in the database when needed.
  - Put key-value returns the old value : this is helpful for rollbacks and trie-logs.




## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 23:04:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    ENH: returning old leafNode on value update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR makes a small but useful modification to the putVisitor.
It is very useful for the trie-log to be able to do the following within a single tree-traversal:
on updating an existing value, retrieve also the old value.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 15:12:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    ADD: implements StoredVerkleTrie
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR adds a new StoredVerkleTrie class representing a VerkleTrie where Nodes can be fetched from storage as needed while walking through the Trie.

Currently, there is a SimpleVerkleTrie which can be constructed in memory only, and there is a StoredNodeFactory which can retrieve a single node from storage. However, there was no mechanism to walk a VerkleTrie where nodes are stored in storage. StoredVerkleTrie fills this gap.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 09:56:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    update gradle for publish step, and MAINTAINERS.md and cleaning of th…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->

## PR description

Cleaning repo (adding maintainers, update gradle for publish etc)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 09:23:44 +0000 UTC
    </div>
</div>

