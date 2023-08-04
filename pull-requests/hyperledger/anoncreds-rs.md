---
layout: default
title: anoncreds-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-rs
---

# anoncreds-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/229" class=".btn">#229</a>
            </td>
            <td>
                <b>
                    Update to anoncreds-clsignatures 0.2, update tails access
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This merges some changes to the tails file handling from indy-credx: the tempfile library is not compatible with some filesystems like on Azure (https://github.com/hyperledger/indy-shared-rs/issues/21). This removes that dependency and adds buffering to the IO operations which helps performance.

The tails file path is no longer required for the credential revocation config when issuing, this would require a JS wrapper update as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 21:03:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/228" class=".btn">#228</a>
            </td>
            <td>
                <b>
                    refactor: services function signatures improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is based on #226 .

Small improvements to the `services` module function signatures aiming to make it easier for native consumers to use the library.

Main goal was to get rid of `TryInto<T, Error = ValidationError>` like arguments because that prevented consumers from passing `T` as an argument (because `TryFrom<T> for T` has an `Infallible` error type).

There still are arguments like `&HashMap<&SchemaId, &Schema>` which aren't really straight-forward to fix due to the implications this has in the FFI layer (maps are constructed at runtime from FFI objects references).

Worth looking into would also be `issuer::update_revocation_status_list()` as it's fairly painful to deal with, but I believe that's really more due to the `RevocationRegistryDelta` - `RevocationStatusList` data structures being different and `anoncreds-clsignatures-rs` using the former.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 14:36:02 +0000 UTC
    </div>
</div>

