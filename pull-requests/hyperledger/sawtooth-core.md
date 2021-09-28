---
layout: default
title: sawtooth-core
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-core
---

# sawtooth-core <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-core){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2400" class=".btn">#2400</a>
            </td>
            <td>
                <b>
                    Remove explicit use of MerkleLeafIterator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the use of `MerkleLeafIterator` as the type of the iterator, as this is an implementation detail not specified in the contract for the `MerkleRadixTree::leaves` function.  The return value is a dynamic boxed iterator.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 16:32:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2399" class=".btn">#2399</a>
            </td>
            <td>
                <b>
                    Serialize message outside for loop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                a slight optimization which prevents the same operation in case
we broadcast to a large number of peers.

Signed-off-by: Alex Todorov <alex.todorov@gluwa.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 14:52:58 +0000 UTC
    </div>
</div>

