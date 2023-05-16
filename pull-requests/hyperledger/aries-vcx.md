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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/844" class=".btn">#844</a>
            </td>
            <td>
                <b>
                    Support referrent-explicit format creating presentation request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - When creating proof request, our API expected list of `<predicate_info>` objects (as they are defined in https://hyperledger.github.io/anoncreds-spec/#create-presentation-request). Aries-vcx implementation then auto-generated referent names, eg given:
```
[
  { name: 'age', p_type: '>=', p_value: 18 }, 
  { name: 'balance', p_type: '>=', p_value: 10000 }
]
```
we transformed the input internally to anoncreds format
```
{
  predicate_0: { name: 'age', p_type: '>=', p_value: 18 }, 
  predicate_1: { name: 'balance', p_type: '>=', p_value: 10000 }
}
```
- This PR enabled API called to simply supply entire `requested_predicates` object (as per anoncreds link above) and therefore letting the caller specify referents names eg.
```
{
  is_adult: { name: 'age', p_type: '>=', p_value: 18 }, 
  credit: { name: 'balance', p_type: '>=', p_value: 10000 }
}
```
This is useful capability when inspecting presentations.

#### Note
- We should remove vector format, it's convenient but not very useful
- String parsing should be happening on layer above `aries-vcx`
- But these are for different PRs

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-14 18:19:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/843" class=".btn">#843</a>
            </td>
            <td>
                <b>
                    Refactor basewallet and corresponding consumers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix: https://github.com/hyperledger/aries-vcx/issues/814

- All JSON strings inputs replaced with rust structs.
- consumers of `BaseWallet` in the code base  updated to use the new types rather than the JSON strings

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-14 16:58:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/842" class=".btn">#842</a>
            </td>
            <td>
                <b>
                    refactor maybe_known.rs: MaybeKnown enum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fixes #839 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-13 07:14:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/840" class=".btn">#840</a>
            </td>
            <td>
                <b>
                    Fix/protocols problem report
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses #835 and #836, essentially adding a `ProblemReport` message to both the `IssueCredential` and `PresentProof` protocols.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 11:55:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/838" class=".btn">#838</a>
            </td>
            <td>
                <b>
                    Split publish_local_revocations in BaseAnoncreds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Splits `publish_local_revocations` method associated with `BaseAnoncreds` trait into `get_rev_reg_delta` and `clear_rev_reg_delta` in order for `IndySdkAnonCreds` to not depend on a `PoolHandle`. Local revocations' publishing is now implemented in an already existing method associated with `RevocationRegistry` which exposes this functionality to the client code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 07:54:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/837" class=".btn">#837</a>
            </td>
            <td>
                <b>
                    Add indy-vdr-proxy profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a new profile `VdrProxyProfile` which uses a running instance of [indy-vdr-proxy](https://github.com/hyperledger/indy-vdr/tree/main/indy-vdr-proxy) (through [indy-vdr-proxy-client](https://github.com/mirgee/indy-vdr/pull/1/files)) to read and write transactions instead of communicating with the ledger directly.

This may be useful in situations where
* a service is limited in its access to the public internet for security reasons or
* the client wants quick and easy access to a ledger without necessarily having to obtain the genesis file and set up and maintain their own ledger connection.

The `VdrProxyProfile` profile reuses existing `IndyVdrLedger` implementation of the `BaseLedger` trait and request submitting is injected through an implementation of the `RequestSubmitter` trait.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 13:03:27 +0000 UTC
    </div>
</div>

