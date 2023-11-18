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
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    FIX: bug in TrieKeyAdaptor swapLastByte
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
There was a bug in TrieKeyAdaptor.swapLastByte : it did not take properly into account the last byte of a UInt256.
Some minor improvements where also made:

  1. UInt256 are reversed to littleEndian as it should be.
  2. All indexes are passed as UInt256.
  3. More tests have been included for contract code chunking.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-17 12:05:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    Chunkify Code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR introduces two new features for TrieKeyAdaptor:

  1. It is now using PedersenHash to generate the keys
  2. It supports code chunkification

This makes it simpler to insert a contract's bytecodes into the trie.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 16:50:06 +0000 UTC
    </div>
</div>

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

