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
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/818" class=".btn">#818</a>
            </td>
            <td>
                <b>
                    Removes references to ~please_ack in other protocols
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `~please_ack` was [recently retired](https://github.com/hyperledger/aries-rfcs/tree/main/features/0317-please-ack). This PR removes the remaining references to `~please_ack` in other protocols. Most relevant to the community is the removal from the issue-credential and present-proof protocols -- which need to be update in AIP 2.0 to include recent clarifications (including this one).

This is not controversial as we have already decided to retire `~please_ack` -- this is just post retirement cleanup.

I think this PR could just be merged with approvals from a @TelegramSam, @TimoGlastra, @genaris but could also wait for an Aries Working Group meeting.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-13 18:12:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/816" class=".btn">#816</a>
            </td>
            <td>
                <b>
                    Clarify issue-credential v2.0 to remove references to payments
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
        Created At 2024-03-11 17:29:17 +0000 UTC
    </div>
</div>

