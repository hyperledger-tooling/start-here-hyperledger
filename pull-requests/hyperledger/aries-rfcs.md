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
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/815" class=".btn">#815</a>
            </td>
            <td>
                <b>
                    Propose reverting issue-credential-v2 and present-proof-v2 to v2.0, removing v2.1 and v2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Proposes that we remove v2.1 and v2.2 from these two protocols, as they are not implemented, v2.1 is not easily implemented (and is an edge case), and makes upgrading to V3.0 harder for anyone that does actually implement them. The bottom line is that as far as we know, no one has implemented these versions, and we want it to stay that way.

To make this change, I copy/pasted the RFCs from those defined in AIP 2.0, and then put in any clarifications that were unrelated to the v2.1 and v2.2 changes.  The result is (I think) an up to date version of each RFC that reflects the reality and direction of the community.

To be discussed at an upcoming Aries Working Group meeting. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 19:05:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/814" class=".btn">#814</a>
            </td>
            <td>
                <b>
                    Update AIP 2.0 to clarified commits, remove some RFCs, retire Please Ack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the definition of AIP 2.0 to update the commits of included RFCs to the latest clarified versions of the RFC, and removes three of the RFCs from the definition of AIP 2.0. Further, the status of one of the removed RFCs (please_ack) is updated to RETIRED, with the background on why it was retired. We'll discuss at a future Aries Working Group call the unchanged "AIP 2.0" in the face of removed RFCs from the Profile. I think, given the state of the AIP, it is acceptable that we do this, given that no one has implemented the removed RFCs.

The full list of categorized changes made are included here, with `DISCUSS` annotations on specific ones to be talked about at an upcoming Aries Working Group call. 

## Updated Commits to AIP 2.0 RFCs -- Status Change to Adopted Only

- [RFC 0005 DIDComm](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0005-didcomm/README.md)
- [RFC 0011 Decorators](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0011-decorators/README.md)
- [RFC 0020 Message Types](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0020-message-types/README.md)
- [RFC 0019 Encryption Envelope](https://github.com/hyperledger/aries-rfcs/tree/main/features/0019-encryption-envelope/README.md)
- [RFC 0025 DIDComm Transports](https://github.com/hyperledger/aries-rfcs/tree/main/features/0025-didcomm-transports/README.md)
- [RFC 0048 Trust Ping](https://github.com/hyperledger/aries-rfcs/tree/main/features/0048-trust-ping/README.md)
- [RFC 0593 JSON-LD Credential Attachment](https://github.com/hyperledger/aries-rfcs/tree/main/features/0593-json-ld-cred-attach/README.md)
- [RFC 0095 Basic Message](https://github.com/hyperledger/aries-rfcs/tree/main/features/0095-basic-message/README.md)

## Updated Commits to AIP 2.0 -- Clarifications

- [RFC 0003 Protocols](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0003-protocols/README.md)
    - Status update to Adopted, Clarifications and additional guidance about the handling of minor differences in protocols by implementations.
- [RFC 0008 Message ID and Threading](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0008-message-id-and-threading/README.me)
    - Status update to Adopted, clarification on having an empty `~thread` on a first message.
- **DISCUSS** [RFC 0627 Static Peer DIDs](https://github.com/hyperledger/aries-rfcs/tree/main/features/0627-static-peer-dids/README.md)
    - Status was recently updated to Retired -- so it makes sense to remove it from the AIP 2.0 list.
    - Update the status line in the RFC to reflect it has been retired.
- **DISCUSSED - Good** [RFC 0519 Goal Codes](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0519-goal-codes/README.md)
    - Added some commonly used Goal Codes
- **DISCUSSED - Good** [RFC 0015 Acks](https://github.com/hyperledger/aries-rfcs/tree/main/features/0015-message-types/README.md)
    - Clarification that an "Ack" value should not be "Fail" and Acks relationship with RFC 0035 Problem Report
- **DISCUSS** [RFC 0023 DID Exchange](https://github.com/hyperledger/aries-rfcs/tree/main/features/0023-did-exchange/README.md)
    - Status update to Adopted, added to example the use of a DID Rotate attachment to include a signature on the the DID
    - Title of the RFC is 1.0, and the version does not seem to have been changed, but there is a reference to a 1.1 version with the DID Rotate.
- **DISCUSSED - Good** [RFC 0035 Report Problem](https://github.com/hyperledger/aries-rfcs/tree/main/features/0035-report-problem/README.md)
    - Clarification that a `description.code` is required, clarification on conventions for warnings
- [RFC 0044 DIDComm File and MIME Types](https://github.com/hyperledger/aries-rfcs/tree/main/features/0044-didcomm-file-and-mime-types/README.md)
    - Clarifications on fallbacks for the mime types and why, and on using JWEs.
- [RFC 0211 Route Coordination](https://github.com/hyperledger/aries-rfcs/tree/main/features/0211-route-coordination/README.md)
    - Adds a comma to the example, correcting a typo.
- [RFC 0434 Out of Band](https://github.com/hyperledger/aries-rfcs/tree/main/features/0434-outofband/README.md)
    - Status update to Adopted, clarification that did:peer:2 can be used for reuse.
- [RFC 0592 Indy Attachments](https://github.com/hyperledger/aries-rfcs/tree/main/features/0592-indy-attachments/README.md)
    - Status update to Adopted, clarification on handling "unrevealed attributes" and clarification on encoding integer strings as numbers (e.g. encoding both `"1"` vs. `1` as integers)
- [RFC 0510 DIF Presentation Exchange Attachment](https://github.com/hyperledger/aries-rfcs/tree/main/features/0510-dif-pres-exch-attach/README.md)
    - Status update to Adopted, correction of reference into the DIF spec that there is an "s" on "definitions" in `dif/presentation-exchange/definitions@v1.0`

## Not Updated

- **DISCUSSED - Good** [RFC 0453 Issue Credential v2](https://github.com/hyperledger/aries-rfcs/tree/main/features/0453-issue-credential-v2/README.md)
    - Status update to Adopted, but applies to v2.2
- **DISCUSSED - Good** [RFC 0454 Present Proof v2](https://github.com/hyperledger/aries-rfcs/tree/main/features/0454-present-proof-v2/README.md)
    - Status update to Adopted, but applies to v2.2

## Removed from AIP 2.0

- **DISCUSSED - Good** [RFC 0587 Encryption Envelope V2](https://github.com/hyperledger/aries-rfcs/tree/main/features/0587-encryption-envelope-v2/README.md)
    - Remove from AIP 2.0 as not needed until we are transitioning to DIDComm V2.
- **DISCUSSED - Good** [RFC 0317 Please ACK](https://github.com/hyperledger/aries-rfcs/tree/main/features/0317-please-ack/README.md)
    - Remove from AIP 2.0 as overly complicated and not helpful. Better to be implemented on a per protocol basis as needed.
    - PR also marks the RFC as "RETIRED" and provides the details about why it was retired, with pointers to the details about a design and code that attempted to implement the functionality, and illustrates why the attempt do not meet the intention of the RFC.

I think leaving the name "AIP 2.0" is acceptable because:

- No one (AFAWK) had implemented the RFCs to be removed.
- Bumping the version would cause more confusion than it is worth.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 17:56:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/813" class=".btn">#813</a>
            </td>
            <td>
                <b>
                    Update index - Feb 2024
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
        Created At 2024-02-15 16:33:52 +0000 UTC
    </div>
</div>

