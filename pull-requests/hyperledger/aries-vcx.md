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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/919" class=".btn">#919</a>
            </td>
            <td>
                <b>
                    Added capability of migrating wallet through the node.js wrapper (#895)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We have previously reverted https://github.com/hyperledger/aries-vcx/pull/906 feature to expose wallet migration in nodejs wrapper. This brings the code back - reverts the revert. 

* Added capability of migrating wallet through the node.js wrapper
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-29 15:56:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/918" class=".btn">#918</a>
            </td>
            <td>
                <b>
                    Refactor features, enable build with --no-default-features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                At high level, this re-enables building aries-vcx, aries-vcx-core without any features enabled. Comes along with some refactoring to make sense of things and prepare ground for gradual removal of vdrtools based components.

- `aries-vcx-core`: define more granular features - this will come handy in subsequent PR's removing parts of vdrtools `vdrtools_anoncreds`, `vdrtools_wallet`, `vdrtools_ledger`
- move non-indy specific files out of indy directories (eg `ToBaseAgencyClientWallet` moved from `aries_vcx_core::wallet::indy::agency_client_wallet` to `aries_vcx_core::wallet::agency_client_wallet`
- `aries-vcx-core`: include `indy-api-types` as dependency to access `indy_api_types::errors` directly to simplify error mapping (`aries_vcx_core/src/errors/mapping_vdrtools.rs` )
- remove support for `vdrtools` based ledger client from `did_resolver_sov` - it was causing some complications which won't be relevant as soon as this https://github.com/hyperledger/aries-vcx/pull/914 get merged

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-28 07:54:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/917" class=".btn">#917</a>
            </td>
            <td>
                <b>
                    Release/0.57.1
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
        Created At 2023-07-27 23:03:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/915" class=".btn">#915</a>
            </td>
            <td>
                <b>
                    Handler layer for SM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ci</span>
            </td>
            <td>
                TODO
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 14:28:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/914" class=".btn">#914</a>
            </td>
            <td>
                <b>
                    Remove vdrtools based ledger client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Delete ledger/pool/zmq related code from vdrtools
- Use `indy-vdr` as ledger client implementation in `aries-vcx`
- Enable setting up Transaction Author Agreement for `indy-vdr` ledger client implementation via `libvcx`
- Disabled libvcx android/ios build jobs - not going to let that hinder progress, created issue to track the problem https://github.com/hyperledger/aries-vcx/issues/916
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 12:39:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/913" class=".btn">#913</a>
            </td>
            <td>
                <b>
                    Allow storing resolvers with varying extra fields in the registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Uses an adaptor which converts the resolved extra fields to a hash map.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 12:27:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/912" class=".btn">#912</a>
            </td>
            <td>
                <b>
                    Modular did:key representation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a struct representing a `did:key`, which can then be used, for example, in the services entries of the OOB invitations or did-exchange requests as per the respective RFCs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 06:57:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/911" class=".btn">#911</a>
            </td>
            <td>
                <b>
                    Move PublicKey to a separate crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows using `PublicKey` in the forthcoming `did_key` crate without importing the entire `did_peer` crate unnecessarily. The only reason `PublicKey` resided in the `did_peer` in the first place was because it was not used anywhere else yet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 15:50:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/910" class=".btn">#910</a>
            </td>
            <td>
                <b>
                    Refactor aries_vcx_core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Small vdrtools adjustment to make indy-wallet compilable without zmq dependency (original intention of PR was to extract wallet out of vdrtools, a strategy I decided to abandon, so this dependency/feature changed in `vdrtools` are here just as "why not" improvement)
- Reorganize files in `aries_vcx_core` such that all wallet APIs are under `aries_vcx_core/wallet` module
- Reorganize `aries_vcx_core` to move files out of `src/indy` into `src/anoncreds` / `src/ledger` / `src/wallet` to keep things together. Previously things been a bit scatter in `src/indy` and other directories. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 10:36:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/909" class=".btn">#909</a>
            </td>
            <td>
                <b>
                    Default to modular libs
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
        Created At 2023-07-24 07:08:47 +0000 UTC
    </div>
</div>

