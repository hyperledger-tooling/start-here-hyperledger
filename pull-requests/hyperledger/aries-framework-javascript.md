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

