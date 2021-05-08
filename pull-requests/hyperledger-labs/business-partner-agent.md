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
                
Changes to UX to load both Material Design and Font Awesome icons, use constants in pages to load the icons. This will allow different teams to just override the value for the constant and have a different icon set.  Also added in a SASS stage to help with changes in styling for each team.

Adding a top level area for managing credentials (issue/revoke). We will need to consider configuration parameters and security roles/groups to enable/disable sections and actions. That is a future task once functionality is implemented.

Have refactored Schema Settings to use the components used in Credential Management / Schema Settings.
Have refactored Partner/Issue Credentials to use the components in Credential Management / Issue Credential.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 18:49:35 +0000 UTC
    </div>
</div>

