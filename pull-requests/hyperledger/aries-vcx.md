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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1126" class=".btn">#1126</a>
            </td>
            <td>
                <b>
                    fix: use selected rust toolchain in ci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Newly installed version of rust toolchain is not used by default: https://github.com/actions-rs/toolchain/issues/210
which leads to error such as https://github.com/hyperledger/aries-vcx/actions/runs/7884528327/job/21520350379?pr=1122

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 14:29:28 +0000 UTC
    </div>
</div>

