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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1498" class=".btn">#1498</a>
            </td>
            <td>
                <b>
                    fix(askar): in memory wallet creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Quick fix to allow the creation of an in-memory wallet (for test purposes). Previously, the parameter was supported but, due to a particular error thrown by `@hyperledger/askar-shared` it was not working.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 22:50:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1496" class=".btn">#1496</a>
            </td>
            <td>
                <b>
                    feat: Create Connection record when receive DidCommV2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Added optional `autoCreateConnectionOnPing` field into Agent config and implemented corresponding logic - indicating whether we should create connection state records when receiving a trust ping message targeted to the DID in the wallet, but with a non-existing pairwise record 
* Updated MessageSender: Unified `sendDidCommV1message` and `sendDidCommV2message` functions into single method `sendMessage`. 
  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 14:41:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1495" class=".btn">#1495</a>
            </td>
            <td>
                <b>
                    fix: race condition singleton records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/aries-framework-javascript/issues/968

This just handles the multiple creation and then erroring of signleton records. 

We still have an issue with multiple writes to the same document, which we should be able to fix with locks
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 12:14:03 +0000 UTC
    </div>
</div>

