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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/858" class=".btn">#858</a>
            </td>
            <td>
                <b>
                    move string parsing to libvcx_core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #845 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-21 13:11:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/857" class=".btn">#857</a>
            </td>
            <td>
                <b>
                    upgrade messages_macros deps to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated message macros dependencies to latest. Fixes #846 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 13:02:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/855" class=".btn">#855</a>
            </td>
            <td>
                <b>
                    In memory response cacher
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implements a simple naive in-memory ledger response cacher and uses it in `IndyVdrLedger`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-18 11:54:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/854" class=".btn">#854</a>
            </td>
            <td>
                <b>
                    Feature/credx issuer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                TODO
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-18 10:27:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/853" class=".btn">#853</a>
            </td>
            <td>
                <b>
                    Remove dependency on BaseWallet from IndyVdrLedger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove dependency on `BaseWallet` from `IndyVdrLedger` in favor of injecting a singing-specific trait implementation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-18 09:03:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/852" class=".btn">#852</a>
            </td>
            <td>
                <b>
                    Implement txn endorsing for IndyVdrLedger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implements `endorse_transaction`, `set_endorser` and `get_txn_author_agreement` for `IndyVdrLedger` and enables `test_endorse_transaction` test.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-18 06:55:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/851" class=".btn">#851</a>
            </td>
            <td>
                <b>
                    Ledger response parser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Extracts ledger response parsing capability into the `indy-ledger-response-parser` crate which
* returns types from `indy-data-types` (reexported by `indy-vdr`) and
* defines its own types (taken from `libvdrtools`) for ledger responses.

This crate is further integrated into `IndyVdrLedger` implementation to replace the current provisional constructions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 10:07:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/850" class=".btn">#850</a>
            </td>
            <td>
                <b>
                    Rename crates: did_doc_builder->did_doc; rename diddoc->diddoc_legacy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Preliminary renaming ahead of https://github.com/hyperledger/aries-vcx/issues/849

Rationale
- `did_doc` seem more suitable named than `did_doc_builder`, as building is 1 part of the crate, but most importantly the crate contains data model for ddo
- you might want to use diddoc without necessary using builder portion of the crate
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-16 11:12:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/848" class=".btn">#848</a>
            </td>
            <td>
                <b>
                    Issue #847: Prover Handler Types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #847 
TODO
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 13:45:28 +0000 UTC
    </div>
</div>

