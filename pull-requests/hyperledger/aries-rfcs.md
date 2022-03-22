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
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/726" class=".btn">#726</a>
            </td>
            <td>
                <b>
                    fix: force the connection into a complete state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When connecting, a race connection can be created. Some invitees will process messages out of order, and a connection may not be in a state that is ready to receive additional messages. The work around is to sleep for an estimated number of seconds. This may cause connectivity issues between invitee and the inviter, and a poor experience in the community.

The recommendation is to change the language so that the invitee MUST send a message to complete the connection, so the inviter may know when it can send additional messages.

Signed-off-by: Kim Ebert <kim@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-21 18:43:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/725" class=".btn">#725</a>
            </td>
            <td>
                <b>
                    Remove Signatures from Example Requests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sam Curren <telegramsam@gmail.com>
These were never appropriate, but added by mistake to the request. Sigs still required in Responses.
Related to #717 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 00:18:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/724" class=".btn">#724</a>
            </td>
            <td>
                <b>
                    Update AIP 2.0 links to point to clarified RFCs -- notably refs to main branch
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
        Created At 2022-03-16 22:04:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/723" class=".btn">#723</a>
            </td>
            <td>
                <b>
                    Update AIP Diff script to use main branch
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
        Created At 2022-03-16 19:06:17 +0000 UTC
    </div>
</div>

