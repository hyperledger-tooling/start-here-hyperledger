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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/409" class=".btn">#409</a>
            </td>
            <td>
                <b>
                    Credential Management/Issuer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backend</span><span class="chip">frontend</span>
            </td>
            <td>
                Draft only right now.

Changes to UX to load both Material Design and Font Awesome icons, use constants in pages to load the icons. This will allow different teams to just override the value for the constant and have a different icon set.  Also added in a SASS stage to help with changes in styling for each team.

Adding a top level area for managing credentials (issue/revoke). We will need to consider configuration parameters and security roles/groups to enable/disable sections and actions. That is a future task once functionality is implemented.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 18:49:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/408" class=".btn">#408</a>
            </td>
            <td>
                <b>
                    Feature/367 frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-01 10:06:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/407" class=".btn">#407</a>
            </td>
            <td>
                <b>
                    Feature/proof request auto-response by bpa (Part 1)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backend</span>
            </td>
            <td>
                BPA satisfies the `auto-respond-presentation-request` acapy flag behaviour and constructs the first valid response available and replies immediately. 

Work-in-progress frontend to see pending proof requests, but none will exist in that due to the current auto-responding implementation. 

This a partial PR that includes alot of the meat of the backend work.

TODO:
- [] handle get pending query params
- [] cleanup (and maybe rename) ProofManager.presentProof. 
- [] handle predicates in the proof-request
- [] Add tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 23:34:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/406" class=".btn">#406</a>
            </td>
            <td>
                <b>
                    Feature/367 frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Allow to manually accept connection requests in the frontend
* Show connection state in partner table
* Added switch to show/hide invitations
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 08:29:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/405" class=".btn">#405</a>
            </td>
            <td>
                <b>
                    Fix bug during transform of CredDef and SchemaAPI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Not sure why this was working before some updates in the pom 🤷‍♂️ . Also noticed that I had to add annotation to my enumerated types in models... that was also working previously.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 19:41:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/404" class=".btn">#404</a>
            </td>
            <td>
                <b>
                    upgrade java to version 16
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                if there aren't any objections i would like to push the java version up to 16
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 12:46:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/403" class=".btn">#403</a>
            </td>
            <td>
                <b>
                    updated to latest micronaut versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 10:51:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    Replaces Feature/connect to personal wallets #399
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 14:46:47 +0000 UTC
    </div>
</div>

