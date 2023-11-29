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
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    TEST: genesis stateroot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Provides a new testcase based on kaustinen genesis.
It puts a list of key-value pairs from a csv file and commits.
The expected stateroot is taken from geth dotfile after genesis.
This can be used to investigates the bugs found in the commitments.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 15:37:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Fix chuckify PUSH32 at 31st byte edge case
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->

## PR description
This PR adds a check to prevent the first byte of a code chunk (push data) to be of value 32 (0x20).
When a PUSH32 appears in the 31 byte of a code chunk (suppose codechunk n) code chunk n+1 should have the first byte declaring that the following 31 bytes are pushdata and codechunk n+2 will have the first byte declaring that the following 1 byte is the overflow of the pushdata.

Test for this has been added using the sample from Kaustinen genesis.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #14 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 05:35:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    WIP: call nativeLib only with BE bytes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-25 17:10:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    Implement `toDot` Method and File Storing Mechanism for `VerkleTrie`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes https://github.com/neotheprogramist/besu-verkle-trie/issues/3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 07:56:46 +0000 UTC
    </div>
</div>

