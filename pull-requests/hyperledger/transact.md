---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/335" class=".btn">#335</a>
            </td>
            <td>
                <b>
                    Stabilize state-merkle-sql-caching by removing it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change stabilizes the "state-merkle-sql-caching" feature by removing it.  This means that the caching capability is available by default with the use of the "state-merkle-sql" feature.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 22:10:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/334" class=".btn">#334</a>
            </td>
            <td>
                <b>
                    Add RUSTFLAGS="-D warnings" to 'just build' 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 21:00:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/333" class=".btn">#333</a>
            </td>
            <td>
                <b>
                    Use const values for hard-coded cache defaults
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Within the implementation, adding const moves the special values to the
top of the module; also adds some doc comments and gives the values
a name.

Within the tests, the const values help differentiate between two
numbers which are provided as parameters next to each other.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 20:38:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/332" class=".btn">#332</a>
            </td>
            <td>
                <b>
                    Add doc to a couple fields in SqlMerkleStateBuilder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Document these two fields because this is quite possibly the first place
these values will be encountered, if one is reading the source top-down.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 20:37:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/331" class=".btn">#331</a>
            </td>
            <td>
                <b>
                    Backport 0-4: Implement state traits v2 for kv::MerkleState
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #328 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-03 16:28:56 +0000 UTC
    </div>
</div>

