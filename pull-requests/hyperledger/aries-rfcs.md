---
layout: default
title: aries-rfcs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-rfcs
---

# aries-rfcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-rfcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/792" class=".btn">#792</a>
            </td>
            <td>
                <b>
                    Goal Code for a flow that simulates a connectionless present proof using a connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Per the addition to the goal codes list -- useful when you want to do a connection-less present proof using a QR code, but the OOB message is too large for the QR code, and URL shortening is not an option.  With this, establish the connection, do the present proof protocol, and delete the connection.

@jleach @cvarjao 

BTW -- not sure where is the best place to create a repository of goal codes to use.  We should discuss that as part of the review of this PR.

Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-08 00:09:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/791" class=".btn">#791</a>
            </td>
            <td>
                <b>
                    Update Index file
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
        Created At 2023-07-06 00:11:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/790" class=".btn">#790</a>
            </td>
            <td>
                <b>
                    Update the AIP 2.0 RFC links to include clarifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A number of RFCs that are part of AIP 2.0 have been updated with clarifications, and this PR updates the links in AIP 2.0 to point to the commits of the clarified versions.  Includes a list of the newly clarified RFCs, and a link to the change made for each one.

I did not include changes to the following RFCs that are part of AIP 2.0:

- 0453 Issue Credential v2.0: The update to RFC included minor version updates, not just a clarification (multiple issuances, supplements)
- 0454 Present Proof v2.0: The update to RFC included minor version updates, not just a clarification (multiple issuances, supplements)
- 0592 Indy Attachments: I think the change that was done (proposed by me...) is wrong and needs to be corrected.

In the list of changes to the links, I've included a link to the PR that added the clarification.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 00:09:13 +0000 UTC
    </div>
</div>

