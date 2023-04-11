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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/797" class=".btn">#797</a>
            </td>
            <td>
                <b>
                    Remove deps in `aries-vcx`: `env_logger`, `android_logger`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - `aries-vcx` should not specify `log` implementation, removed `env_logger` as well as android build dependency `android_logger`
- similar changes in other crates as well
- added `env_logger` to `vcx-napi-rs` along with its initialization (same as previously in `aries-vcx`) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 07:41:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/796" class=".btn">#796</a>
            </td>
            <td>
                <b>
                    Remove unnecessary dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Removed unused dependencies across the board
- `vdrtools`: Remove unused ffi wallet declarations (in `libvdrtools/indy-api-types/src/lib.rs`) and unsupported function for wallet plugin registration `register_wallet_storage`
- Removed commented tests in vdrtools
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 20:13:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/794" class=".btn">#794</a>
            </td>
            <td>
                <b>
                    Remove proof verifier legacy format deserialization support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - As planned in https://github.com/hyperledger/aries-vcx/pull/770 next release won't support legacy format of serialized verifier proofs. 

- Follow migration guide in the PR linked above using aries-vcx `0.53.0` to reserialize your verifier proofs to the new format. The next `aries-vcx` release `0.54.0` will not support non-migrated verifier proofs created by `aries-vcx` `0.52.x` or older.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 17:41:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/793" class=".btn">#793</a>
            </td>
            <td>
                <b>
                    Add get_revocation_id for IssuerCredential
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
        Created At 2023-04-06 08:28:46 +0000 UTC
    </div>
</div>

