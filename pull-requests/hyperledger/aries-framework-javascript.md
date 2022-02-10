---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/632" class=".btn">#632</a>
            </td>
            <td>
                <b>
                    fix: leading zeros in credential value encoding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR resolves an interop issue between ACA-Py & AFJ—in credential issuance we verify that the credential did not change between what was offered and what is actually being issued. 

If the credential attribute value to be encoded (as described [here](https://github.com/hyperledger/aries-rfcs/blob/be4ad0a6fb2823bb1fc109364c96f077d5d8dffa/features/0036-issue-credential/README.md#encoding-claims-for-indy-based-verifiable-credentials)) is a string of numbers that contains a leading zero, such as an account number like: `08888`, then ACA-Py removes the leading zero (`8888`), while AFJ instead encodes it with the zero (`08888`). This PR adjusts AFJ’s behavior to bring it in line with ACA-Py’s implementation.

Signed-off-by: James Ebert <jamesebert.k@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 18:25:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/631" class=".btn">#631</a>
            </td>
            <td>
                <b>
                    feat: update recursive backoff & trust ping record updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Supersedes #458 and incorporates discussions there.
This PR alters the logic for trust pings so that connection records are not updated and events emitted if the record is already in a 'Complete' state.
Fixes the recursive mediator reconnection backoff behavior

Signed-off-by: James Ebert <jamesebert.k@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 17:56:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/630" class=".btn">#630</a>
            </td>
            <td>
                <b>
                    Feat/present proof v2
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
        Created At 2022-02-08 13:21:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/629" class=".btn">#629</a>
            </td>
            <td>
                <b>
                    Issue credv2
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
        Created At 2022-02-08 13:17:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/628" class=".btn">#628</a>
            </td>
            <td>
                <b>
                    merge changes
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
        Created At 2022-02-08 10:10:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/627" class=".btn">#627</a>
            </td>
            <td>
                <b>
                    Issue credv2
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
        Created At 2022-02-08 10:02:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/626" class=".btn">#626</a>
            </td>
            <td>
                <b>
                    fix: check for "REQNACK" response from indy ledger 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solves #569 

Signed-off-by: annelein <anneleinvanreijen@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 15:39:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/625" class=".btn">#625</a>
            </td>
            <td>
                <b>
                    fix: credential preview attributes mismatch schema attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solves #587 

TO DO:
- [ ] Write tests

Signed-off-by: annelein <anneleinvanreijen@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 13:02:06 +0000 UTC
    </div>
</div>

