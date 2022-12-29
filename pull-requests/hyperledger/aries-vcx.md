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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/711" class=".btn">#711</a>
            </td>
            <td>
                <b>
                    Libvcx/minimize api c
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Improvements in libvcx triggered working on https://github.com/hyperledger/aries-vcx/pull/665


- make feature `libvcx_c` default
- minimize responsibility of `api_c` - move logic of reading `CONFIG_INSTITUTION_DID` from `api_c` to `api_vcx`
- change FFI signature of `vcx_credentialdef_create_v2` by removing its `issuer_did: *const c_char` argument - this is inconsistent with all the other APIs which load the did from setting `CONFIG_INSTITUTION_DID`
- shorten test `test_release_all` 
- do not return unnecessary `error::SUCCESS_ERR_CODE` codes from `api_vcx` layer - this was a leftover of past where today's `api_c` and `api_vcx` were tied much closer together
- all `update_state*` methods in `api_vcx` return new state on success
- reuse state value returned by `update_state` in `update_state*` methods in `api_c`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-29 11:11:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/710" class=".btn">#710</a>
            </td>
            <td>
                <b>
                    Libvcx/refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Divides `libvcx` in 2 main `api_c` and `api_vcx` modules which could be potentially split out as separate crates https://github.com/hyperledger/aries-vcx/issues/700
- `api_c` depends on `api_vcx` and contain libvcx c interface
- `api_vcx` doesn't know about `api_c` and contains the internal logic
- This should make implementation on https://github.com/hyperledger/aries-vcx/pull/665 smoother
- `errors` module was moved under `src/errors` to be consistent with other crates (previously under `src/api_lib/errors`)
- Defined build feature `libvcx_c` - if specified, `api_c` is included in the build

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-27 18:58:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/708" class=".btn">#708</a>
            </td>
            <td>
                <b>
                    Draft: CredxAnoncreds verifier functionality support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #699 Implements credx verifier method and tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-23 12:52:15 +0000 UTC
    </div>
</div>

