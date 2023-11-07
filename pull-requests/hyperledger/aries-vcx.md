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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1051" class=".btn">#1051</a>
            </td>
            <td>
                <b>
                    fix(did_parser): Add readme and simple example (#1047)
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
        Created At 2023-11-06 15:44:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1046" class=".btn">#1046</a>
            </td>
            <td>
                <b>
                    Feature/did exchange additions
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
        Created At 2023-11-06 00:22:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1043" class=".btn">#1043</a>
            </td>
            <td>
                <b>
                    Enhance `aries_vcx` crate readme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Rewrote `aries_vcx` crate readme
- Rename `aries-vcx` package to `aries_vcx`, looking at most of are other crates, it seems that underscore is "the way" :-) I like it though

Also want to point out the distinction between `aries-vcx` and `aries_vcx`:
- `aries-vcx` being name of the HL project currently containing variety of useful components, not particularly tied to aries itself - such as crates `did`, `did_doc`, `did_peer` and number of others
- `aries_vcx` is the main, but also just one of many crates in the repo
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 17:26:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1042" class=".btn">#1042</a>
            </td>
            <td>
                <b>
                    Raw draft of refactored primitives interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PoC redesign of `Wallet`, `Ledger` and `Vc`(`Anoncreds`) traits.

The `Wallet` and `Ledger` traits were split an designed to work with the `WalletRecord` and `LedgerRequest` traits.

The `WalletRecord` and `LedgerRequest` traits are meant to be implemented on data types that would convert to/from an associated type for the `Wallet` or `Ledger` respectively, enabling the interfaces to work with multiple sets of VC data structures, for instance.

The `Anoncreds` trait is split on roles into `VcIssuer`, `VcVerifier` and `VcProver`. Strong typing and associate types have been added for them.

The `Vc` traits are meant to work with the `Wallet` and `WalletRecord` and have some intense trait bounds that essentially allow a couple of things:
- the ability to store a record in the wallet.
- the ability to retrieve a record from the wallet using the designated ID.
- conversion/linkage between ID data types for the `Wallet` and `WalletRecord` that enables the things above.

There are some compile time tests for the `VcIssuer` implementation for `indy` to ensure that the traits and their extreme trait bounds are actually usable from consumer code. (`VcVerifier` is very simple).

**NOTE**: The trait bounds were a lot of work and involved a lot of trial and error. It's possible some could be removed without affecting the code functionality. Feel free to experiment, as the compiler will surely yell at you if something needed is removed 😅 .

**IMPORTANT**: While this is sort of replicating the `credx` implementation for verifiable credentials, it must be reviewed and refactored to use more static typing here and there, as well as ensuring it does the proper thing as some stuff was removed as part of adding strong types for arguments.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 14:28:59 +0000 UTC
    </div>
</div>

