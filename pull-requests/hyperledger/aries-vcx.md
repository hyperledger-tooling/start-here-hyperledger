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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/767" class=".btn">#767</a>
            </td>
            <td>
                <b>
                    Expose getting and clearing attributes from the ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">wrappers</span>
            </td>
            <td>
                Expose functions getting and clearing value of the latest attribute transaction for the specified did through the node wrapper API.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 08:01:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/766" class=".btn">#766</a>
            </td>
            <td>
                <b>
                    Update sqlx version to 0.6.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                update sqlx version
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 23:27:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/765" class=".btn">#765</a>
            </td>
            <td>
                <b>
                    Release 0.53.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 22:48:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/764" class=".btn">#764</a>
            </td>
            <td>
                <b>
                    Rename prover methods, extend test test_generate_self_attested_proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## API changes (in `aries-vcx`, `libvcx_core`, `vcx-napi-rs`)
#### proof (verifier) methods:
- `presentation_request(...)` renamed to `presentation_request_msg(...)`
- `presentation(...)` renamed to `get_presentation_msg(...)`
- `presentation_status(...)` renamed to `get_presentation_status(...)`
- `get_proof_state(...)` renamed to `proof_get_presentation_verification_status(...)`
- in `libvcx_core` and upwards added methods: `get_presentation_attachment(...)`, `get_presentation_request_attachment(...)` - these are returning decoded versions of attachment in the respective messages (json as string)

#### disclosed proof methods:
- `generate_proof_msg(...)` renamed to `get_presentation_msg(...)` (it's not generating anything, probably did historically)

## NodeJS
#### NodeJS wrapper
- Removed `getProof(...)` which combined 2 ffi calls removed
- instead added granular api `getPresentationMsg(...)`, `getPresentationVerificationStatus(...)`, `getPresentationAttachment(...)`

###  vcxagent-core
- generalized testing util method `sendHolderProof(...)` to make proofData injectable, updated tests
- fixed various standard warnings
- added test `Faber should verify proof with self attestation`
- Added asserts to existing proof tests to check verification status and inspect values received in the received presentation

### Testing
- Extended test `test_generate_self_attested_proof ` to include verification of proof containing of self-attested attributes

- method renames in `libvcx_core`
  - `generate_proof_msg(...)` -> `get_presentation_msg(...)`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 17:05:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/763" class=".btn">#763</a>
            </td>
            <td>
                <b>
                    Experiment - Vdrtools as a feature flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is mostly just an experimental proof of concept to put all aries-vcx usages of libvdrtools under a feature flag (which aries-vcx has as a default flag).

The idea is that consumers who do not want to use vdrtools dependencies (e.g. using modular deps or their even own deps instead), can override the default flag and use their own `Profile`. This way the consumer does not have to pull in the heavy-weight deps of libvdrtools

I imagine once the modular deps (i.e. issuer&verifer & askar-wallet) implementations are fleshed out, we would have a feature flag for those implementations as well, and then importing consumers can toggle between what they wish to use.


# Other Changes
There are still some usages of `crate::indy` splatter around the codebase that need to be isolated. Specifically, `LibIndyMocks`, which could probably just become a more general `GlobalMocks` structure, or something like that. I'm yet to work this out.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 14:05:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/762" class=".btn">#762</a>
            </td>
            <td>
                <b>
                    OOB invite attachment field conditional serialization, default to empty if not present
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span><span class="chip">breaking</span><span class="chip">skip-ios</span><span class="chip">skip-android</span><span class="chip">skip-napi-m1</span>
            </td>
            <td>
                Currently:

* deserialization of OOB invitation fails if `requests~attach` field is not present, and
* when no messages were attached to OOB invitation, the attachments field serializes to an empty vec unnecessarily.

This change:

* sets default value for the field to fix the first issue, and
* skips serialization if the attachments are empty to fix the second issue.

This is a breaking change: prior versions of aries-vcx are not forward compatible with this change and fail to deserialize OOB invitations without `requests~attach` field. However, after this change, aries-vcx is still backwards compatible with OOB invitations produced by earlier versions of aries-vcx.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 19:35:51 +0000 UTC
    </div>
</div>

