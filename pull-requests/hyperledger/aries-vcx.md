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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/771" class=".btn">#771</a>
            </td>
            <td>
                <b>
                    Sort error mapping by numeric code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Correctness verified by existing tests `it_should_map_error_kinds_to_codes` and `it_should_map_error_codes_to_error_kinds`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 20:27:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/770" class=".btn">#770</a>
            </td>
            <td>
                <b>
                    Changed Proof (Verifier) API for checking presentation status
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Short summary
- Changes to Proof (verifier) API
- Backward compatible changes `0.53.0`, however won't be anymore in the subsequent release `0.54.0` - however migration is straightforward

## Changes `aries-vcx`
- Function `fn presentation_status(&self) -> Status` removed - it returned a result as a combination of revocation status and aries state.
- Function 
```
fn get_revocation_status(handle: u32) -> LibvcxResult<VcxRevocationStatus>
```
 replaced by new
 ```
 fn get_presentation_status(&self) -> PresentationVerificationStatus
 ``` 
semantically returning the same result.

Other way to look at it is that `get_revocation_status()` was removed and `presentation_status() / get_presentation_status()` was changed to yield similar result as `get_revocation_status` did.


### Changes `aries-vcx` Internals
- Replace `RevocationStatus` enum by new enum `PresentationVerificationStatus`.
   - The enum values are more accurately reflecting the actual nature of things - when presentation is verified, we only know whether the presentation is valid/invalid https://github.com/hyperledger/aries-vcx/blob/main/aries_vcx/src/protocols/proof_presentation/verifier/state_machine.rs#L225 (and yes, revocation can be common cause of invalidity, but not necessarily the only one - it can be simply buggy prover or a malicious actor tweaking the proof) 
- The new `PresentationVerificationStatus` is backwards compatible, so there's a mapping of old values such as `Revoked` to new value `Invalid` etc. 
- The verifier's `FinishedState` previously maintained the information as `Option<RevocationStatus>` whereas now it keeps `PresentationVerificationStatus` and the new enum contains variant `Unavailable`, so we don't need the `Option`. This makes it bit nicer to work with as there's less destructuring
   - Again, for sake of backwards compatibility, `null` or missing value will deserialize to `PresentationVerificationStatus::Unavailable`
- Renamed field `revocation_status` to `verification_status`, however also enable deserialization from the original`revocation_status` to enable backward compatibility

## Changes `libvcx_core`
- Changes analogously propagated from `aries_vcx` eg.
  - Removed `get_revocation_status`
  - Behaviour of `get_presentation_verification_status ` changed, as this function now simply returns value of `PresentationVerificationStatus` (as opposed to previous convoluted behaviour of that function).
  
## Changes`libvcx`, ios+java wrappers
- Modified function `vcx_get_proof_msg` so it returns presentation message as the name suggests (removed value of `get_presentation_verification_status ` from the result tuple)

## Migration
This slightly changes format of serialized (Verifier) Proof state machines, however still supports old format for reading in the next release `0.53.0`. The support for reading serialized Proof created before `0.53.0` will be dropped in `0.54.0`. If you wish to maintain ability to these older state machines, you will need to re-serialize state machine with `0.53.0` release, eg. (example in JS)
```
let vcxProofSerialized = await someStorage.load("proof123") // load the proof created by VCX before 0.53.0
let vcxProof = Proof.deserialize(vcxProofSerialized) // the 0.53.0 is still able to deserialize the old format
let reserialized = vcxProof.serialize() // serialized into new format
await smeStorage.save("proof123", reserialized) // stores the new format
```

## Summary of the API after changes:
Forgetting about the delta, this is the final state:
Verifiers' Proof has 2 main methods to determine state
- `pub fn get_state(&self) -> VerifierState` - returns the Aries state from enum:
```
Initial
PresentationProposalReceived
PresentationRequestSet
PresentationRequestSent
Finished
Failed
```

- `pub fn get_verification_status(&self) -> PresentationVerificationStatus` - returns state of presentation verification, which can be one of following variants:
```
Valid - presentation was verified and valid
Invalid - presentation was verified, but was not valid (common cause can be using revoked credential in presentation)
Unavailable - no presentation is available to verifier
```




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-13 16:08:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/769" class=".btn">#769</a>
            </td>
            <td>
                <b>
                    Proof verifier: add `get_revocation_status` method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - In nodejs wrapper, rename `ProofStatus` to `ProofVerificationStatus`
- Add `get_revocation_status` to `libvcx_core` to find out revocation status of verifier's proof state machine, expose to nodejs wrapper
- Note: `RevocationStatus` is `aries-vcx` structure which in `libvcx_core` maps to `VcxRevocationStatus`, which includes numeric mappings. This is to avoid polluting `aries-vcx` with numeric encoding
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 22:48:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/768" class=".btn">#768</a>
            </td>
            <td>
                <b>
                    Draft: Apply Typestate pattern to Holder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                TODO...

To determine:
* Approach for legacy `Holder` support? - should this replace the existing or be a new construct?
* How to handle state transitions which previous result in two different state?.. e.g. `Holder<OfferReceived>::send_request` could progress into `Failed` or `RequestSent` according to the old API
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 09:03:12 +0000 UTC
    </div>
</div>

