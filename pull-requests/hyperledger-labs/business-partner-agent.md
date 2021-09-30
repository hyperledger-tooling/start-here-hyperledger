---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/640" class=".btn">#640</a>
            </td>
            <td>
                <b>
                    The Org Name/Agent Name needed alignment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/640"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 22:46:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/639" class=".btn">#639</a>
            </td>
            <td>
                <b>
                    value not needed.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Sy <jasyrotuck@gmail.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/639"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 20:44:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/638" class=".btn">#638</a>
            </td>
            <td>
                <b>
                    Proof Template: Allow multiple restrictions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - addresses https://github.com/hyperledger-labs/business-partner-agent/issues/637 it is now possible to add one or many restrictions to a proof request
- error events are now handled on both sides (holder, verifier), so we now see if the proof request was illegal. This can happen for example when there are two credentials in the wallet one with name=10, and one with name=MyName and we send a proof request requesting name to be < 11. In this case aca-py logs an error and ends the proof request immediately.
- schema version and schema name are not pre-filled any more
- the backend truncates trusted and schema issuer dids if they are fully qualified, as aca-py only allows the last segment of the did at the moment for proof requests v1
- fixed bug in the credential component

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/638"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 15:10:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/636" class=".btn">#636</a>
            </td>
            <td>
                <b>
                    Public Profile layout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Put Org Profile and Creds in cards.
Allow user to jump directly to edit Org. Profile (requested from UAT).
Users were getting lost when they clicked on Public Profile and then couldn't edit their Organization name, compromise by adding direct jump to that edit form.  The edit button should be protected by RBAC in the future.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

![Screen Shot 2021-09-24 at 3 52 27 PM](https://user-images.githubusercontent.com/39388115/134748518-7e5e1d82-a9ff-46c1-9c7e-e6057ceadcd3.png)


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/636"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 23:17:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/633" class=".btn">#633</a>
            </td>
            <td>
                <b>
                    Fix: save credential data if auto-respond-credential-proposal is set to true
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
        Created At 2021-09-23 15:42:51 +0000 UTC
    </div>
</div>

