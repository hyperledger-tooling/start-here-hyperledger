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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 14:31:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/928" class=".btn">#928</a>
            </td>
            <td>
                <b>
                    DID Exchange Protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Initial version of [DID Exchange protocol](https://github.com/hyperledger/aries-rfcs/blob/main/features/0023-did-exchange/README.md#request-message-attributes) implementation with support for peer DIDs (peer:did:2 for now), new `DidDocument` crate, and JWS signing / verification.

The primary aim is not to achieve perfection at this stage but to roll out a first iteration prototype.

Correctness has been tested (so far only) using AATH tests running against AcaPy peer:did branch (or against aries-vcx itself), where all didx tests are passing whether the requester or responder role is assumed by either side.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 12:06:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/927" class=".btn">#927</a>
            </td>
            <td>
                <b>
                    Use credx anoncreds in napi wrapper
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
        Created At 2023-08-09 22:47:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/925" class=".btn">#925</a>
            </td>
            <td>
                <b>
                    Remove init_issuer_config function
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
        Created At 2023-08-05 18:00:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/924" class=".btn">#924</a>
            </td>
            <td>
                <b>
                    fix(aries-vcx): fixed dependency listing in README for `Cargo.toml`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using path does not work and crates from git sources need be specified through `git=...`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-04 17:38:38 +0000 UTC
    </div>
</div>

