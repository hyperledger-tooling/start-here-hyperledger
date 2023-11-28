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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1650" class=".btn">#1650</a>
            </td>
            <td>
                <b>
                    refactor: move message-pickup directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For some strange reason, the 'i' in `message-pickup` module directory is an special character, which makes it difficult to create patches to properly test updates in that module (like the ones in #1638), so this small PR is just fixing it using a regular 'i'.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-27 12:23:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1648" class=".btn">#1648</a>
            </td>
            <td>
                <b>
                    refactor(anoncreds)!: move supportRevocation to options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This moves the `supportRevocation` option in the registerCredentialDefinition method to the `options` object. It feels a bit weird to me that we have an `options` object, but then not place an option like `supportRevocation` in that options object

@genaris you ok with this change?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-27 03:58:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1647" class=".btn">#1647</a>
            </td>
            <td>
                <b>
                    feat!: allow to query tenant records using label
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Requested by someone in the discord
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 05:38:49 +0000 UTC
    </div>
</div>

