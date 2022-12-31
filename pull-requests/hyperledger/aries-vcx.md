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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/714" class=".btn">#714</a>
            </td>
            <td>
                <b>
                    Minor renames, remove unnecessary asyncs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Additional sequel to https://github.com/hyperledger/aries-vcx/pull/711 refactoring

- removed `async` where no `await` was actually used
- renamed 2 functions within `api_vcx` libvcx layer 


Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-31 17:16:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/713" class=".btn">#713</a>
            </td>
            <td>
                <b>
                    Clippy do not allow unwrap used
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Denies clippy rule defined here: https://rust-lang.github.io/rust-clippy/master/#unwrap_used

ideally we should be not panicking at all (unless testing). however in some places where it's obvious an error will not occur (e.g. some `lazy_static` variable blocks), we will use `.expect(...)` instead - knowing that the `expect` should never occur.

Note that also in some places, where we know it is only used for testing (e.g. mocks) `expect`s are used - this may be changed in the future if desired.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-30 14:57:24 +0000 UTC
    </div>
</div>

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
- change FFI signature of `vcx_credentialdef_create_v2` by removing its `issuer_did: *const c_char` argument - this is inconsistent with all the other APIs which load the did from setting `CONFIG_INSTITUTION_DID` - technically a breaking change, but holistically the argument didn't have usecase, nobody should be impacted.
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

