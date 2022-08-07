---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/974" class=".btn">#974</a>
            </td>
            <td>
                <b>
                    feat: Action Menu protocol (Aries RFC 0509) implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implementation of module fully supporting [Aries RFC 0509](https://github.com/hyperledger/aries-rfcs/blob/main/features/0509-action-menu/README.md) for both `requester` and `responder` roles.

Protocol states and information are stored in records of type `ActionMenuRecord`. As this protocol currently defines a single active menu per connection, there will be at most 2 records per connection (as theoretically is possible to serve as requester and responder at the same time). While this information could be stored also in Connection Metadata, specific records were created thinking in a future version/extension of this protocol where multiple menus could be deployed (e.g. a menu by thread).

Still plenty of tests to do and fixes/support for error messages, as well as check compatibility with ACA-Py implementation.

Solves #471 
Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-06 23:42:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/972" class=".btn">#972</a>
            </td>
            <td>
                <b>
                    feat(proofs): Present Proof as nested protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As exemplified in [Aries RFC 0008](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0008-message-id-and-threading#nested-example), there are certain situations where proofs must be exchanged as part of an inner flow, such as a credential issuance.

This PR attempts to support launching a Present Proof V1 protocol as a sub-protocol from another one, without impacting current Agent behaviour and API (apart from adding some fields and methods). It does not, however, add support for all threading concepts (such as `sender_order` and `receiver_order`), as it might introduce breaking changes and also needs to be more carefully designed.

Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 19:42:09 +0000 UTC
    </div>
</div>

