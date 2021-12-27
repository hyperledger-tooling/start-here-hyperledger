---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    Decouple generating and sending credential offer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Built on top of https://github.com/hyperledger/aries-vcx/pull/419

This is somewhat revert, as I am adding `OfferSet` state which we have previously removed. Consequently send_offer transition became quite "fat" as it was conveniently performing 2 steps:
- generating libindy credential offer
- sending aries credential offer message to counterparty

However this is not always desirable, and in particular doesn't work for OOB workflows. To issue OOB credential, I need to strictly build credential offer and message delivery can happen via arbitrary communication channel. 

This RP replaces 
```
pub fn send_credential_offer(&mut self, offer_info: OfferInfo, comment: Option<&str>, send_message: impl Fn(&A2AMessage) -> VcxResult<()>) -> VcxResult<()>
```
with primarily
```
pub fn build_credential_offer_msg(&mut self, offer_info: OfferInfo, comment: Option<String>) -> VcxResult<()> 
pub fn mark_credential_offer_sent(&mut self) -> VcxResult<()> 
pub fn get_credential_offer_msg(&self) -> VcxResult<CredentialOffer>
```
and temporarily I also kept `send_credential_offer` but became rather a "convenience function" and probably can be removed soon.
```
pub fn send_credential_offer(&mut self, send_message: impl Fn(&A2AMessage) -> VcxResult<()>) -> VcxResult<()>
```

New version of `send_credential_offer` is backward compatible and preserves functionality.
For new OOB flows, it's expected to:
- call `build_credential_offer_msg`
- call `get_credential_offer_msg` to get aries credential offer message
- wrap the credential offer in OOB message
- deliver the OOB message the receiver 
- call `mark_credential_offer_sent`
- wait for credential request with matching thread_id and progress the issuance protocol

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-27 17:13:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    Issuer SM stores aries cred offer instead of libindy offer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Issuer state machine stores generic Aries Credential Offer message, rather than specific libindy offer structure. 
- Libindy offer structure is needed to issue indy credential, hence upon issuance, libindy structure is retrieved from Aries Cred Offer attachment - it's assumed the attachment is libindy offer.

This is one of small steps towards decoupling Aries FSM layer and libindy.

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-27 10:47:55 +0000 UTC
    </div>
</div>

