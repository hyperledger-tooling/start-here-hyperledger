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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/679" class=".btn">#679</a>
            </td>
            <td>
                <b>
                    feat: Regex for schemaVersion, issuerDid, credDefId, schemaId, schemaIssuerDid
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
        Created At 2022-03-23 13:51:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/678" class=".btn">#678</a>
            </td>
            <td>
                <b>
                    fix: added logic for further inbound message val
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added IsEncrypted message, and changed logic so we do not just assume message is agent message (i.e. error message)
TODO: In future we could add error event emitter for this type of error, rather than throwing AriesFrameworkError

Signed-off-by: Niall Shaw <niall.shaw@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 15:29:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/677" class=".btn">#677</a>
            </td>
            <td>
                <b>
                    fix: do not use basic message id as record id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This makes it impossible to send a basic message to yourself
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-21 20:11:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/676" class=".btn">#676</a>
            </td>
            <td>
                <b>
                    feat: Replace old oob invitation with the new one
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I removed all use of `ConnectionInvitationMessage` inside the framework, it is used only in the conversion method from the "old" oob to the "new" one. And also in tests for unused methods, I would like to look at them if I can reuse some tests cases for the new methods.

I also refactored a bit mediation `provision` method by splitting making a connection and requesting mediation as we discussed on the call yesterday.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 11:46:33 +0000 UTC
    </div>
</div>

