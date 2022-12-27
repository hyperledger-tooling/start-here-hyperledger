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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/703" class=".btn">#703</a>
            </td>
            <td>
                <b>
                    Code formatting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fail CI if code is not correctly formatted
- Adjusted `rustfmt.toml` to bit more liberal setup from its default `max_width=100` to `max_width=120` - however given `use_small_heuristics` https://rust-lang.github.io/rustfmt/?version=v1.5.1&search=#use_small_heuristics most of the lines will be well below 120 characters.
- Applied reformat
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 10:18:39 +0000 UTC
    </div>
</div>

