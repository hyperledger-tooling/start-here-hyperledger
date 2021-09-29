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
                https://github.com/hyperledger-labs/business-partner-agent/issues/637

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/632" class=".btn">#632</a>
            </td>
            <td>
                <b>
                    Bcgov wording
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                tried templating everything, but started to see more cost than gains, some typo style things i changed for everyone. Other more specific words are delegated to the template. 

Too many changes to capture them all, but we are focusing on providing context for an audience that is not familiar with the app rather than use the most correct terminology that we (the developers) would use. 

If this is too much clutter, we could put this in our own fork if that is preferred. 



<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/632"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 00:18:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/631" class=".btn">#631</a>
            </td>
            <td>
                <b>
                    Connection by Invitation Activity Log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Was creating a task when connecting by connection invitation that couldn't be closed.
Was not creating an activity log when connection by oob invitation.

Now, we just create an activity log when the connection is "complete" in both the `c_i` and `oob` invitations.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/631"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 22:09:13 +0000 UTC
    </div>
</div>

