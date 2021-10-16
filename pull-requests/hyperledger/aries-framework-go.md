---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3012" class=".btn">#3012</a>
            </td>
            <td>
                <b>
                    feat: OOB create/accept invitation commands use accept/mediatypeprofile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                CreateInvitation:
- Add accept parameter to command
- If accept parameter not present, use agent's first MediaTypeProfile.
  If agent doesn't have any MediaTypeProfile set, default to the aip2 rfc19
  profile, as before.

AcceptInvitation:
- use agent's media type profiles to validate oob accept handshake

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 23:02:39 +0000 UTC
    </div>
</div>

