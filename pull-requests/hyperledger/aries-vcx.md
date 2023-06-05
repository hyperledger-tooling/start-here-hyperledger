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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/869" class=".btn">#869</a>
            </td>
            <td>
                <b>
                    Extend Profile trait with update_taa_configuration method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In PR https://github.com/hyperledger/aries-vcx/pull/863 we have eliminated global state used by modular profile. However:
- we didn't have way to set up TAA in runtime without having to rebuild entire Profile
- that was manifested by `ModularLibsProfile` having fields with `public(crate)` visibility so we could accommodate different initialization flow which needs indy writer with TAA (also resulting in some code duplication in `aries_vcx/src/utils/devsetup.rs`)
- equally we would run into hiccups when we integrate `ModularLibsProfile` with `vcx-napi-rs` and try sync up  implementation for `set_active_txn_author_agreement_meta`


This PR introduces interior mutability within `ModularLibsProfile` such that it's possible to update TAA setup for ledger writer in runtime - doing so by wrapping the `anoncreds_ledger_write`, `indy_ledger_write` in `RwLock` - note these wrapped trait objects are the same instance under the hood.

As RwLocks has been added wrapping the ledger write trait objects, in order to prevent having to modify codebase across many files and deal with locks everywhere, obtaining locks has been encapsulated into `IndyLedgerWriteProxy`, `AnoncredsLedgerWriteProxy` which implement `IndyLedgerWriteProxy`, `AnoncredsLedgerWriteProxy` respectively. This enabled us to introduce RwLocks without surrounding code consuming Profile trait being aware of it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 09:30:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/868" class=".btn">#868</a>
            </td>
            <td>
                <b>
                    Minor DDO service builder improvement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use the typestate pattern to statically ensure service type was set.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 13:32:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/867" class=".btn">#867</a>
            </td>
            <td>
                <b>
                    Feature/cred migrator
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
        Created At 2023-06-01 15:51:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/866" class=".btn">#866</a>
            </td>
            <td>
                <b>
                    Refactor messages crate tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix: #822 

Just want to know that the direction in which I'm going is upright! For using the `Static JSON` in message crate tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 13:57:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/865" class=".btn">#865</a>
            </td>
            <td>
                <b>
                    Make DidDocument's service generic over method-specific fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As it was decided that `DidDocument` integration will be postponed, this PR cherry-picks those changes made in #864 which are isolated to the new crates and thus can be merged independently from the `DidDocument` integration.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 13:27:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/864" class=".btn">#864</a>
            </td>
            <td>
                <b>
                    WIP: DidDocument integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">breaking</span><span class="chip">integration</span>
            </td>
            <td>
                Replaces the use of
* `diddoc_legacy::aries::diddoc::AriesDidDoc` with `did_doc::schema::did_doc::DidDocument`, and
* `diddoc_legacy::aries::service::AriesService` with `did_doc::schema::service::Service`
across the aries-vcx codebase.

Integration with mediated connection is skipped and `diddoc_legacy` will be removed along with `mediated_connection`.

The method specific fields of the service struct are now set via a type associated with the `DidResolvable` trait, where only fields specific to the sovrin method are used in the codebase for now. This choice impacts the current implementation of the resolver registry, which needs to be reconsidered.

Moreover, currently, the service type is set manually during the construction of the `DidDocument`, and the `accept` field is not set at all. However, as per the [Sovrin DID method specification](https://sovrin-foundation.github.io/sovrin/spec/did-method-spec-template.html#crud-operation-definitions), the value of those two fields is implied by the composition of / fields included in the service. This suggests that potentially we might want to wrap the `DidDocumentBuilder` in some kind of `DidDocumentBuilderSov` responsible for this method-specific logic in the future.

This would be also useful because the extra fields are defined in `did_resolver_sov`. In some use-cases, the entire resolver is imported only for the extra fields needed in order to name the `DidDocument` or `Service` type.

The DID parser fails to parse any did which is not fully qualified. This is desirable in cases where fully qualified DID is required as it forces early failure. But in situations where the method is implied, an unqualified DID may also be valid and usable. Therefore, perhaps a separate type should be created to be used in these cases.

As it stands, this integration is a breaking change as it changes the format of the `did_doc` field in the serialized connection state machines in both non-backwards-compatible and non-forwards-compatible way (e.g. some fields optional in the legacy format are now required and `publicKey` used in the legacy format is not a valid DDO field - it can probably be mapped to another valid field when deserializing, but currently isn't).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 18:12:50 +0000 UTC
    </div>
</div>

