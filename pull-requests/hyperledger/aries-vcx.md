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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/908" class=".btn">#908</a>
            </td>
            <td>
                <b>
                    Specify default libvcx feature flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fix build for libvcx ios/java artifacts (no features flags are selected for ios/java builds, will fail in runtime)
- fail on compile if no implementation is selected via feature flags
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-23 15:41:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/907" class=".btn">#907</a>
            </td>
            <td>
                <b>
                    testing/remove-mixed-breed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                One less thing to worry about - since "mixed breed" testing profile was introduced, we have increased coverage with different profile significantly, and also introduced 4x different testing combinations on `libvcx_core` level. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 13:08:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/906" class=".btn">#906</a>
            </td>
            <td>
                <b>
                    Revert "Added capability of migrating wallet through the node.js wrap…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit be57e49e5fb15c790e68d8f060e8328922a7e7a1 / https://github.com/hyperledger/aries-vcx/pull/895

The PR is causing CI to fail, because it added migrator as dependency of `libvcx_core`. The migrator imports `ariesvcx_core` with `modular_libs` feature, I believe that's the culprit of the issues - as both vdrtool and indyvdr become part of the build - altough seems to work with major scenarios, in tests etc, there are probably some interplay of dependencies during the build process when building for ios/android/linux musl (napi wrapper build)

Strategic way to go about this is to to default to `indy-vdr` ledger client, delete vdrtools based ledger client (and therefore the zmq dependencies coming from `vdrtools`) and then re-apply the changes in reverted commit. 
That might solve the issue, or at least make it simpler to investigate.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 12:48:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/905" class=".btn">#905</a>
            </td>
            <td>
                <b>
                    Build artifacts with indy-vdr as ledger client
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
        Created At 2023-07-21 12:36:39 +0000 UTC
    </div>
</div>

