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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/861" class=".btn">#861</a>
            </td>
            <td>
                <b>
                    Split BaseLedger trait
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                Splits `BaseLedger` trait into smaller ones:
* `AnoncredsLedgerRead` - methods for resolving Anoncreds primitives
* `AnoncredsLedgerWrite` - methods for registering Anoncreds primitives
* `IndyLedgerRead` - methods for reading Indy-specific transactions from the ledger
* `IndyLedgerWrite` - methods for writing Indy-specific transactions to the Ledger

Among other things, this allows eventual elimination of TAA stored in global state by building the "reader" which allows to obtain the TAA from ledger and use said TAA to construct a "writer" which needs TAA to write to the ledger.

The associated methods `set_endorser` and `endorse_transaction` may stand out:
* The method `set_endorser`, temporarily associated with `IndyLedgerRead`, does not read from the ledger, but merely modifies a transaction.
* The method `endorse_transaction`, temporarily associated with `IndyLedgerWrite`, again only manipulates an existing transaction (adds a multisignature) before submitting.
The pattern with the remaining methods is that a ledger-specific request is built from scratch using the supplied data and submitted to the ledger. Perhaps therefore, local modification of existing requests should not be the responsibility of mentioned traits.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 05:19:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/860" class=".btn">#860</a>
            </td>
            <td>
                <b>
                    Remove vcx_schema_prepare_for_endorser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                Removes:
* `sign_and_submit_request` from `BaseLedger`
* `build_schema_request` from `BaseLedger`
* `vcx_schema_prepare_for_endorser` from `api_c`
* `test_vcx_endorse_schema` test
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 12:06:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/859" class=".btn">#859</a>
            </td>
            <td>
                <b>
                    Release 0.56.0
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
        Created At 2023-05-22 14:12:27 +0000 UTC
    </div>
</div>

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
                This PR completes the credx anoncreds implementation by adding proper handling for issuer operations. For tests, the `mixed_breed` feature flag was added (with teary eyes, since we want to get rid of them not add more) so that a new profile can be constructed.

The mixed breed profile uses the credx anoncreds impl and the indy ledger and wallet impls.
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

