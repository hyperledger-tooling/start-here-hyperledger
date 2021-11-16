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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1494" class=".btn">#1494</a>
            </td>
            <td>
                <b>
                    Fix TypeError
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When calling /schemas/{schema_id}/write_record, a server error 500 occurrs. The log output says

    TypeError: inject() got an unexpected keyword argument 'required'

Other code in this file seems to indicate that the proposed change is what is needed to prevent the error from being thrown.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 12:37:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1493" class=".btn">#1493</a>
            </td>
            <td>
                <b>
                    DIF PresExch - ProblemReport and "is_holder"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1486 
- review all tests involving `TEST_CRED_DICT` and `TEST_CRED_WILDCARD` with `FHIR` contexts to mock `pyld` returns.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 20:56:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1492" class=".btn">#1492</a>
            </td>
            <td>
                <b>
                    Aries Cloud Agent Python Release 0.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 18:38:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1491" class=".btn">#1491</a>
            </td>
            <td>
                <b>
                    DIF PresExch Tests - temporary update to fix pyld.jsonld.JsonLdError
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a repeat of #1251 , then it started working without any updates after sometime.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 17:10:08 +0000 UTC
    </div>
</div>

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

