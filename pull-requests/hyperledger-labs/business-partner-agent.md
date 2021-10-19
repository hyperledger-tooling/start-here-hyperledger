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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/658" class=".btn">#658</a>
            </td>
            <td>
                <b>
                    Small wording changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Presentation Request accepted -> Proof has been sent
Organization profile now has an edit button, so remove instructions to go to the edit page. 

Signed-off-by: Jason Sy <jasyrotuck@gmail.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/658"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 18:17:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/657" class=".btn">#657</a>
            </td>
            <td>
                <b>
                    Schema Attribute RegEx change.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                schemas with capital letters and/or mixed case cause errors on credential comparison/match

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/657"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 22:05:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/656" class=".btn">#656</a>
            </td>
            <td>
                <b>
                    Badge on Notifications only.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #630 

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/656"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 23:00:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/655" class=".btn">#655</a>
            </td>
            <td>
                <b>
                    Option to handle credential offer manually
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
        Created At 2021-10-15 15:37:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/654" class=".btn">#654</a>
            </td>
            <td>
                <b>
                    Selected Credential not being used in backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change the API to not use aca-py models, don't try fulfill aca-py request directly.
Small fix on view credential exchange when you are a holder and haven't stored the schema.

fixes #634 
 
Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/654"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 22:49:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/652" class=".btn">#652</a>
            </td>
            <td>
                <b>
                    New Presentation Exchange Modal, View completed one
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Needed to redo this from a different branch base 

Only visible when viewing finished presentation exchanges. 

Signed-off-by: Jason Sy <jasyrotuck@gmail.com>


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/652"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 18:43:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/651" class=".btn">#651</a>
            </td>
            <td>
                <b>
                    Merge Credential Issuer And Holder Tables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As a prerequisite for the manual credential proposal flow I had to merge the issuer and holder tables into one. Like this we have the same behavior as with the presentation flows. So in the ui the user will also see the credentials that have been received from a partner, and not only those that were issued.

<img width="1183" alt="Screen Shot 2021-10-13 at 17 30 34" src="https://user-images.githubusercontent.com/13498217/137165405-0a9fb709-0990-45fa-b585-c73afc9f9d62.png">


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/651"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 15:27:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/648" class=".btn">#648</a>
            </td>
            <td>
                <b>
                    Partner Select List bug - remove Invitations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also remove from dashboard counts and do not include in the chat message list.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/648"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 19:50:16 +0000 UTC
    </div>
</div>

