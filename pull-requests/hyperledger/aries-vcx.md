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

EDIT: Found [this](https://github.com/TimoGlastra/legacy-did-transformation) document. This implementation should (eventually) follow the described algorithm.
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/934" class=".btn">#934</a>
            </td>
            <td>
                <b>
                    Eliminate dependence of indy-ledger-response-parser on indy-api-types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Eliminates dependence of `indy-ledger-response-parser`  on `indy-api-types`, which now leak out of `libvdrtools` only through `indy-wallet`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-11 13:23:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/932" class=".btn">#932</a>
            </td>
            <td>
                <b>
                    Rebuild cargo.lock, restore indy-vdr-proxy txn submitter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - used `indy-vdr` dependencies with following fix https://github.com/mirgee/indy-vdr/pull/2/file
- rebuilt lock file

It seems due to issue in the `indy-vdr-proxy-client` cargo.toml file, it was bringing in wrong `indy-vdr` version and then our dependency tree ended up with 2 versions of indy-vdr. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 17:36:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/931" class=".btn">#931</a>
            </td>
            <td>
                <b>
                    Updated indy-credx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #926 .

This introduces yet another feature flag, `legacy_proof`, because after a lot of digging the proof request and verification appear to change in credx in a way that's not backwards compatible. However, the feature flag enables a second check of the proof using the legacy method.

This is not the default behavior because people might not want to have this enabled at all times.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 14:31:17 +0000 UTC
    </div>
</div>

