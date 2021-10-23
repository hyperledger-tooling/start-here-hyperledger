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
                PR <a href="https://github.com/hyperledger/transact/pull/229" class=".btn">#229</a>
            </td>
            <td>
                <b>
                    Update rust docs for sabre protocols
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 21:26:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/228" class=".btn">#228</a>
            </td>
            <td>
                <b>
                    Add release notes for 0.3.12
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
        Created At 2021-10-21 20:18:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/227" class=".btn">#227</a>
            </td>
            <td>
                <b>
                    sabre protocol doc typo fixes
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
        Created At 2021-10-21 19:33:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/226" class=".btn">#226</a>
            </td>
            <td>
                <b>
                    Fix typo in doc comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 19:25:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/225" class=".btn">#225</a>
            </td>
            <td>
                <b>
                    Backport 0-3: Multi-threaded bug fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backports PR #222 into 0-3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 19:31:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/224" class=".btn">#224</a>
            </td>
            <td>
                <b>
                    Fix typo in rustdoc for SabreContext.add_receipt_data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 17:55:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/223" class=".btn">#223</a>
            </td>
            <td>
                <b>
                    Backport 0-3: Limit recursion to same tree ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Back-port of #221 to 0-3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 16:38:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/222" class=".btn">#222</a>
            </td>
            <td>
                <b>
                    Multi-threaded bug fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a test for multi-threaded reads using merkle state implementations.  This test identified several issues with the SqlMerkleState sqlite and postgres implementations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 01:26:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/221" class=".btn">#221</a>
            </td>
            <td>
                <b>
                    Limit recursion to same tree ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change limits the SQL recursion to the same tree_id.  This prevents an issue where the existence of multiple trees with duplicate structure creates an infinite loop in SQLite.

The same change has been applied to the recursive queries in Postgres.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 15:27:12 +0000 UTC
    </div>
</div>

