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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/863" class=".btn">#863</a>
            </td>
            <td>
                <b>
                    Remove reliance of IndyVdrLedger on global state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                Makes `ProtocolVersion` and `TxnAuthrAgrmtAcceptanceData` injectable to `IndyVdrLedgerRead` and `IndyVdrLedgerWrite` on construction, thus removing their reliance on global `settings`. Also:
* adds TAA ledger response parsing, and
* `get_txn_author_agreement` now returns `VcxCoreResult<Option<String>>` instead of `VcxCoreResult<String>` - however all getter methods should follow the same pattern.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 13:48:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/862" class=".btn">#862</a>
            </td>
            <td>
                <b>
                    Split IndyVdrLedger and IndySdkLedger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                Splits 
* `IndyVdrLedger` -> `IndyVdrLedgerRead` & `IndyVdrLedgerWrite`, and
* `IndySdkLedger` -> `IndySdkLedgerRead` & `IndySdkLedgerWrite`

This allows each implementation to use only what it needs (e.g. `IndyVdrLedgerRead` variant doesn't need `RequestSigner`, `IndyVdrLedgerWrite` doesn't need `ResponseCacher` and `ResponseParser`). Moreover, since both are initialized separately, a `IndyLedgerRead` implementation can be used to initialize a `IndyLedgerWrite` implementation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 10:55:30 +0000 UTC
    </div>
</div>

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

