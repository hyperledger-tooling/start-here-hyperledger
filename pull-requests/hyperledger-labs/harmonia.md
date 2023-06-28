---
layout: default
title: harmonia
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/harmonia
---

# harmonia <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/harmonia){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/harmonia/pull/39" class=".btn">#39</a>
            </td>
            <td>
                <b>
                    Test proof of inclusion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added test that proves event was generated from a transaction that was actually included in a block.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 12:13:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/harmonia/pull/37" class=".btn">#37</a>
            </td>
            <td>
                <b>
                    Update README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix ERC 721
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 16:06:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/harmonia/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    Refactor to clarify path logic and simplify node creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR does the following:

* Represents the "nibble array" concept in EVM's path encoding using a dedicated class, `NibbleArray`, which provides a range of methods for querying and manipulating paths, and translating between nibble and byte array representations.
* Represents the prefix logic in EVM's path encoding using a pair of enums, `PatriciaTriePathType` and `PatriciaTriePathPrefix`.
* Assimilates the different `Node` subclasses to inner classes of `Node`, and makes `Node` itself a sealed class.
* Rationalises the ways a `Node` can be created, so that everything uses the standard set of methods supplied in `Node`'s companion object.
* Removes boilerplate in test cases by introducing some helpful builder functions for populating tries and constructing trees of nested `Node`s.

The overall intention is to improve code readability and reduce ambiguity (when is this `ByteArray` really an array of bytes, and when is it an array of nibbles?).

A shortcoming of Kotlin 1.2.17 appears to be that members of sealed classes can only be defined as inner classes of the sealed class, which makes `Node` a little cumbersome.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 15:43:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/harmonia/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    [FEAT] Patricia Merkle Trie
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a new implementation of Patricia Merkle trie with support for proofs generation and verification.
Added test for new Patricia Merkle trie implementation.

Updated README.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 12:57:46 +0000 UTC
    </div>
</div>

