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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1131" class=".btn">#1131</a>
            </td>
            <td>
                <b>
                    fix: specify a tag for napi-rs image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                should fix https://github.com/hyperledger/aries-vcx/actions/runs/8000705387/job/21850571000
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-22 07:41:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1130" class=".btn">#1130</a>
            </td>
            <td>
                <b>
                    Type requested credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `requested_credentials_json` is now passed to `prover_create_proof` as a dedicated type instead of `&str`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 15:06:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1129" class=".btn">#1129</a>
            </td>
            <td>
                <b>
                    feat: add workflow for building napi images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a workflow that should build and pushe updated napi image.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 12:04:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1128" class=".btn">#1128</a>
            </td>
            <td>
                <b>
                    Remove impl_anoncreds_object_identifier macro
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 07:07:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1127" class=".btn">#1127</a>
            </td>
            <td>
                <b>
                    refactor: remove ProofRequestData
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                After adding the `anoncreds_types` crate, some types defined in `aries-vcx` are now being duplicated. This set of changes removes `ProofRequestData`.

Moreover:
* Removed `RevocationRegistryDelta` "primitive" struct
* Removed unused `RevocationDetails`
* Removed `CredentialDefConfig` to avoid confusion with a similar struct in `anoncreds_types`
* Removed `update_state` method of `Schema` "primitive", a preliminary step to removing the struct altogether
* Removed unused errors from `anoncreds_types`
* Removed `ConversionError` and `ValidationError` from `anoncreds_types`
* Pruned `anoncreds_types::Error`

- [x] Add tests for the non-legacy restrictions / predicates format
- [x] Proper `PresentationRequest` versioning
- [ ] Custom(ized) builder for `PresentationRequest` (?)
- [x] Handle errors resulting from Nonce creation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 09:09:02 +0000 UTC
    </div>
</div>

