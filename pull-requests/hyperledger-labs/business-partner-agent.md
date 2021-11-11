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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/670" class=".btn">#670</a>
            </td>
            <td>
                <b>
                    Display build number in settings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - cleaned up delombok a bit, but it is not working -> duplicate class error, needs different paths, but as we are not shipping a javadoc jar I skipped this for now
- added option to set Maven .jar version from the build pipeline
- removed obsolete smart tag action from the build pipeline and replaced it with the metadata action
- version of the jar should be either sha or tag (in that order), but needs running on main to be sure, otherwise we need to fallback to the revision of the commit
- added build version und uptime to the UI settings section

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/670"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 14:57:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/669" class=".btn">#669</a>
            </td>
            <td>
                <b>
                    Feature/UI polish: Decline with reason
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Different changes to improve the Partner UI and exchange tables:

- Credential exchange dialog: Add text field to send an optional decline reason message
- Presentation exchange dialog: Add text field to send an optional decline reason message
- Display reason message as tooltip on decline icon
- Display reason message in timelines in dialogs
- Change missing trusted issuer warning to info (colors)
- Add text in addition to icon on revoked status in table
- Improve icon height in tables
- Capitalize some texts for consistency

Dev stuff:

- Add local docker tails server for development in local scenario
- Adapted .env example file

![image](https://user-images.githubusercontent.com/87176157/140942113-d9487b88-1155-4c5f-a751-fff1f9a2719b.png)
![image](https://user-images.githubusercontent.com/87176157/140942370-cb16eef2-0836-4a2e-916e-60cf8241cb24.png)
![image](https://user-images.githubusercontent.com/87176157/140942502-1aa482ae-8b6c-40f7-9576-c1db9560a1a0.png)
![image](https://user-images.githubusercontent.com/87176157/140942582-cf0f447d-cc1c-46a1-bc1d-a6308adc415c.png)


<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/669"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 14:30:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/668" class=".btn">#668</a>
            </td>
            <td>
                <b>
                    Disable auto respond credential request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is about fixing some remaining issues in the exchange states.

1. Store credential information on credential issued (only v2, not implemented in v1), as the acked event is only a courtesy and might not be implemented by all agents.
2. Disable auto respond credential request flag. This one is a bit tricky as in v1 indy a credential request event is always preceeded by an offer, so here we can always auto respond because the user has already accepted the offer. Whereas in v2 a holder can initiate the flow directly. This means running an agent with this auto flag enabled results in auto issuance, which could be a security issue when running none test bpa instances. So I changed the behaviour in the v2 handler that credential requests without a prior offer are denied. We can implement this flow later for v2, which is a nice shortcut feature.
3. Verry basic proof request name resolution. when receiving v1 proof proposals
4. Auto accepting crredential offer when offer == proposal, otherwise manual acceptance is required
5. Added v2 option to request verification flow



Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/668"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 13:41:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/667" class=".btn">#667</a>
            </td>
            <td>
                <b>
                    fixing holder revocation states in partner details
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/667"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 09:54:09 +0000 UTC
    </div>
</div>

