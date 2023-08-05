---
layout: default
title: aries-framework-javascript-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript-ext
---

# aries-framework-javascript-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/223" class=".btn">#223</a>
            </td>
            <td>
                <b>
                    fix(push-notifications)!: align to RFCs 0699/0734
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates Push Notifications modules to support all features mentioned in Aries RFCs [0699](https://github.com/hyperledger/aries-rfcs/tree/main/features/0699-push-notifications-apns) (for APNS) and [0734](https://github.com/hyperledger/aries-rfcs/tree/main/features/0734-push-notifications-fcm) (for FCM).

There are only two changes in the API for both mechanisms:
- `deviceInfo()` now needs an additional parameter, because to create a `device-info` message it's needed to specify the threadId (as it is generated as a response for a `get-device-info` message)
- `DeviceInfo` data can now accept both `string` and `null`

This adds some basic error handling, like throwing a Problem Report in case that either device_token or device_platform are null. Maybe it could be interesting in a further PR to add records (or use Connection Metadata) to do automated responses and more checks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-05 14:11:36 +0000 UTC
    </div>
</div>

