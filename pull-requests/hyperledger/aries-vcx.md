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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/710" class=".btn">#710</a>
            </td>
            <td>
                <b>
                    Libvcx/refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Divides `libvcx` in 2 main `api_c` and `api_vcx` modules which could be potentially split out as separate crates https://github.com/hyperledger/aries-vcx/issues/700
- `api_c` depends on `api_vcx` and contain libvcx c interface
- `api_vcx` doesn't know about `api_c` and contains the internal logic
- This should make implementation on https://github.com/hyperledger/aries-vcx/pull/665/files smoother
- `errors` module was moved under `src/errors` to be consistent with other crates (previously under `src/api_lib/errors`)
- Defined build feature `libvcx_c` - if specified, `api_c` is included in the build

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-27 18:58:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/708" class=".btn">#708</a>
            </td>
            <td>
                <b>
                    Draft: CredxAnoncreds verifier functionality support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #699 Implements credx verifier method and tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-23 12:52:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/705" class=".btn">#705</a>
            </td>
            <td>
                <b>
                    CI: Add clippy checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - some exceptions were granted for now, eg. allowing lints which are by default a warning - see top of `lib.rs` of respective crates
- removing this exceptions will be separate task(s) (can be easy task for new contributors perhaps)
- various warnings fixed

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 22:45:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/704" class=".btn">#704</a>
            </td>
            <td>
                <b>
                    Refactor diddoc, extract as crate, create crate vcx_shared
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note: The commits in these PR are quite well separated, might we worthy to review commit-by-commit approach

This PR is further addressing https://github.com/hyperledger/aries-vcx/issues/697

Changes:
- Aries/w3c diddoc divergence
   - Added `W3cDidDoc` - this reflects https://www.w3.org/TR/did-core/#example-30-did-document-with-1-verification-method-type but is not currently used anywhere as there's a slight divergence due aries `service` extensions.
   - Renamed original `DidDoc` to `AriesDidDoc` 
   - The difference between the 2 is most of all `service` attribute - the rendered diddoc resolved by `did:sov` has an extra attributes like `recipientKeys`, `routingKeys` etc. (see `Resolver DID Document Format` @ https://sovrin-foundation.github.io/sovrin/spec/did-method-spec-template.html)
   - Long term we should use `W3cDidDoc` or find better abstraction to fit in the aries stuff
   
- Renamed `ServiceResolvable` - which sounds like and interface but is enum, to `ServiceOob`. This represents either `AriesService` or a DiD, for which AriesService can be resolved from ledger per OOB spec https://github.com/hyperledger/aries-rfcs/blob/main/features/0434-outofband/README.md#messages
   > services - an array of union types that the receiver uses when responding to the message. Each item is either a DIDComm service object (as per [RFC0067](https://github.com/hyperledger/aries-rfcs/blob/main/features/0067-didcomm-diddoc-conventions/README.md#service-conventions)) or a DID (as per [Decentralized Identifiers v1.0](https://w3c.github.io/did-core/#did-syntax)). Additional details below.
   
- Moved `EndpointDidSov` under `aries-vcx/common/ledger` - it has nothing to do with Aries messages, eventually should end up in some DID DOC resolver module
- Added optional field `types` which was missing in `EndpointDidSov` (as specified in `DID Service Endpoint` @ https://sovrin-foundation.github.io/sovrin/spec/did-method-spec-template.html#crud-operation-definitions )
- Extracted all diddoc related code to separate crate - as by itself is more general concept and has no relation to `aries`
- As result, I also ended up creating `vcx_shared` crate to avoid yet another duplication of methods `validate_did` and `validate_verkey`

Built on top of https://github.com/hyperledger/aries-vcx/pull/702
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 15:46:31 +0000 UTC
    </div>
</div>

