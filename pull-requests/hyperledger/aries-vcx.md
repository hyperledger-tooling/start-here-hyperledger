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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/944" class=".btn">#944</a>
            </td>
            <td>
                <b>
                    Proposal/processor
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
        Created At 2023-08-18 16:17:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/943" class=".btn">#943</a>
            </td>
            <td>
                <b>
                    Remove libvcx-c, libvcx java, libvcx ios
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After ~9 months of deprecation, we remove libvcx-c and associated java and ios wrappers.

However, anyone with strong interest to keep this components "alive" is welcome to take owner their ownership and maintenance. Please contact us if you are interested and we can provide some guidance.

However, recommended strategy for mobile devices is building custom FFI layer on top of aries-vcx crate. There's project in progress https://github.com/hyperledger/aries-vcx/pull/896 demonstrating such approaching using UniFFI library. While not complete, it's great starting point for anyone looking to build native, aries enabled, mobile app.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 14:15:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/942" class=".btn">#942</a>
            </td>
            <td>
                <b>
                    Release 0.58.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - First release with removed libvcx-c, libcx java and ios wrappers. See https://github.com/hyperledger/aries-vcx/pull/943
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 14:00:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/941" class=".btn">#941</a>
            </td>
            <td>
                <b>
                    Expose public key getter on verification method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Introduces a `public_key::Key` getter in `VerificationMethod` to facilitate easy retrieval of the key representation derived from `VerificationMethod`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 06:54:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/940" class=".btn">#940</a>
            </td>
            <td>
                <b>
                    Try Hide indy-api-types from modular_libs consumers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Testing...

i _believe_ that modular_libs should not need anything to do with indy-api-types after this great PR: https://github.com/hyperledger/aries-vcx/pull/934, therefore we should make it optional in aries_vcx_core..

this takes the dep count from `554` to `300` for:
```
cargo check --features modular_libs --no-default-features -p aries-vcx
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 09:02:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/939" class=".btn">#939</a>
            </td>
            <td>
                <b>
                    Extract subset of changes made in #928
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Extracts changes made to `did_doc`, `did_doc_sov`, `did_doc_sov`, `did_peer`, and `public_key` crates in #928. Most of these changes are either consequences of #913 or additions of features found to be useful during #928.

The reason for extracting these changes is that
* doing so will minimize conflicts encountered when rebasing #928 after changes made to the modified crates (e.g. in  #938),
* they are independent and useful outside of #928.

TODO: Prune
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-16 10:01:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/938" class=".btn">#938</a>
            </td>
            <td>
                <b>
                    Attempt to convert legacy DID documents to new during deserialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Introduces a lightweight, easy-to-remove legacy DDO data structure to the `did_document_sov` crate. During the deserialization of `DidDocumentSov`, if the incoming data matches the legacy structure, it is converted to `DidDocumentSov` with `IndyAgent` service type.

Received legacy DDO is first converted to did:peer:2 following [this](https://github.com/TimoGlastra/legacy-did-transformation) document, and from it then back-resolved to the new DDO format following the did:peer:2 spec.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-16 07:09:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/937" class=".btn">#937</a>
            </td>
            <td>
                <b>
                    Modify connection inviter to extract msg sending out
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @nain-F49FF806 will soon start integrating connection protocol into mediator service. Since clients connecting to mediator have no inbound endpoint to receive messages on, the clients will need to request transport return route https://github.com/hyperledger/aries-rfcs/blob/main/features/0092-transport-return-route/README.md
to receive aries responses in http responses.
Naian will be using only inviter side of Connection, and it's important the state machine implementation doesn't include response sending.  While `send_response` with some in-memory transport channel could still work to deliver responses, getting rid seems cleaner.
Hence:
- removed `InviterConnection<Requested>::send_response`
- added  `InviterConnection<Requested>::get_connection_response_msg`, `InviterConnection<Requested>::mark_response_sent`

No breaking changes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 21:54:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/936" class=".btn">#936</a>
            </td>
            <td>
                <b>
                    Allow parsing unqualified DIDs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enables parsing of unqualified DIDs in `did_parser`, a temporary measure for the purposes of gracefully transitioning to using fully qualified DIDs, and will be reverted once the transition is complete.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 13:51:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/935" class=".btn">#935</a>
            </td>
            <td>
                <b>
                    Update indy-vdr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update indy-vdr to latest main rev (as it contains `vdr-proxy-client` (unlike any (pre-)release)).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 10:52:03 +0000 UTC
    </div>
</div>

