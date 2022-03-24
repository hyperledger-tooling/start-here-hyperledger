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
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/727" class=".btn">#727</a>
            </td>
            <td>
                <b>
                    Update ACK RFC 0015 to remove FAIL and add reference to using problem-report instead
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR created after a discussion in the [Aries WG Meeting - 20220316](https://wiki.hyperledger.org/display/ARIES/2022-03-16+Aries+Working+Group+Call)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 20:16:30 +0000 UTC
    </div>
</div>

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

