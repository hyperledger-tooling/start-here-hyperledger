---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1945" class=".btn">#1945</a>
            </td>
            <td>
                <b>
                    Update pip-audit.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-17 20:17:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1944" class=".btn">#1944</a>
            </td>
            <td>
                <b>
                    Update pip-audit.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 21:10:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1941" class=".btn">#1941</a>
            </td>
            <td>
                <b>
                    Add startup flag --light-weight-webhook to trim down outbound webhook payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When we create a credential offer with image, the image is repeated in following objects (dict) 
"credential_request", "cred_request", "credential_proposal", "cred_proposal", "credential_offer", "cred_offer", "credential_preview", "cred_preview", "values", "credentials~attach", "offers~attach"

a Credential offer with 30KB image resulted in a webhook sized at 227KB in my use case and resulted HTTP 413 as well as unnecessary stress on WAF rule regex processes on those encrypted string and base64 image string.

This startup flag will remove those objects only on outbound webhook and size went down to 7KB at most.
I did preserve 1 object "cred_issue" which has the "rev_reg_id" and "cred_rev_id".

To me this is a more like a nice to have flag if someone ever encounter problem with image and webhook.

Previous related discussion
[PR #725](https://github.com/hyperledger/aries-cloudagent-python/pull/725)
[Issue #1222](https://github.com/hyperledger/aries-cloudagent-python/issues/1222)

Signed-off-by: Victor Lee <victorlee0505@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 20:48:08 +0000 UTC
    </div>
</div>

