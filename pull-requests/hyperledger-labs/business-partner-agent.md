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
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/672" class=".btn">#672</a>
            </td>
            <td>
                <b>
                    Option to reissue an existing credential if it is in state revoked
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/672"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 15:24:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/671" class=".btn">#671</a>
            </td>
            <td>
                <b>
                    fix jar name in dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/671"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 13:35:30 +0000 UTC
    </div>
</div>

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

