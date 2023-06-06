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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/873" class=".btn">#873</a>
            </td>
            <td>
                <b>
                    Inject only required components, not entire profiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `Profile` abstraction has been introduced to enable smooth transition from `vdrtools` to modular libs (credx/anoncreds, indy-vdr, askar). `Profile` represents basket of trait objects to perform variety of operations.

Previously `Profile` was widely present in `aries-vcx` codebase as a convenient way to access various lower-level APIs. However this was at the price of:
- passing references to objects down the stack, even though they were never used,
- requiring `aries-vcx` consumers to build entire "Profile", even though the APIs they've consequently used only used limited number of profile's components (eg, you don't need access to ledger in order to build credential proposal, for example)
- forcing `aries-vcx` to store building blocks in particular way (Profiles) - but consuming applications might want to store/handle things differntly.

This PR modifies `aries-vcx` and `aries-vcx-core` method signatures to be unaware of `Profile` abstraction - the APIs now only speak in terms of individual components such as `dyn BaseAnoncreds`, `dyn AnoncredsLedgerRead` - so the APIs ask only for what they really need.
Additional extra benefit is that it's now much easier to spot fishy stuff, like "oh, this method requires access to ledger? That's weird, why is that???"


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-06 11:57:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/872" class=".btn">#872</a>
            </td>
            <td>
                <b>
                    Refactor/do not consume profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ios</span><span class="chip">skip-android</span><span class="chip">skip-napi-m1</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-06 11:51:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/871" class=".btn">#871</a>
            </td>
            <td>
                <b>
                    Sovrin-specific DDO facade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Introduces wrappers around `DidDocument` and `Service` in order to
* handle logic specific to the Sovrin method, e.g.
    * setting and validating `type` and `accept` fields based on the composition of the service extra fields,
    * dereferencing service keys (?)
* remove definition of the Sovrin extra fields from `did_resolver_sov`,
* simplify common Sovrin DDO usage patterns (e.g. retrieving recipient / routing key from the first service in the `service` field, etc.).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 15:01:27 +0000 UTC
    </div>
</div>

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
                <span class="chip">skip-ios</span><span class="chip">skip-android</span><span class="chip">skip-napi-m1</span>
            </td>
            <td>
                In PR https://github.com/hyperledger/aries-vcx/pull/863 we have eliminated global state used by modular profile. However:
- we didn't have way to set up TAA in runtime without having to rebuild entire Profile
- that was manifested by `ModularLibsProfile` having fields with `public(crate)` visibility so we could accommodate different initialization flow which needs indy writer with TAA (also resulting in some code duplication in `aries_vcx/src/utils/devsetup.rs`)
- equally we would run into hiccups when we integrate `ModularLibsProfile` with `vcx-napi-rs` and try sync up  implementation for `set_active_txn_author_agreement_meta`

This PR introduces interior mutability within `IndyVdrLedgerWrite` such that it's possible to update TAA setup for ledger writer in runtime
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

