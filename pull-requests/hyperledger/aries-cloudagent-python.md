---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1490" class=".btn">#1490</a>
            </td>
            <td>
                <b>
                    fix: using a default mediator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes an error in the use of a default mediator in the connections and out of band protocols. The mediation ID was being saved as None instead of the retrieved default mediator value.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-13 22:51:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1489" class=".btn">#1489</a>
            </td>
            <td>
                <b>
                    Update to ReadMe and Supported RFCs for 0.7.2.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates to readme to better reflect the current state of ACA-Py. 

Update the "Supported RFCs" doc to use the checklist style that Northern Block and Animo Solutions created.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 22:30:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1488" class=".btn">#1488</a>
            </td>
            <td>
                <b>
                    Updating the RTDs code for Release 0.7.2 - Try 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the the Read The Docs material in preparation for the next release of ACA-Py. We'll leave this as a WIP until 0.7.2 is ready to be released, to catch the latest updates.

There is one error that has been there since 0.7.1 -- not sure the reason or fix.  Anyone?

`WARNING: error while formatting arguments for aries_cloudagent.protocols.issue_credential.v1_0.models.credential_exchange.V10CredentialExchange: unhashable type: 'list'`

I'll keep this open until 0.7.2 is final.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 22:48:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1484" class=".btn">#1484</a>
            </td>
            <td>
                <b>
                    Clarify instructions in Acme Controller Workshop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1477 

Signed-off-by: Elias Strehle <elias@circulartree.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 09:38:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1483" class=".btn">#1483</a>
            </td>
            <td>
                <b>
                    fix: create static doc use empty endpoint if None
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This enables us to use the undelivered queue with static connections by not specifying the endpoint.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 19:58:36 +0000 UTC
    </div>
</div>

