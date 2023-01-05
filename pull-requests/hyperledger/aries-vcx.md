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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/718" class=".btn">#718</a>
            </td>
            <td>
                <b>
                    Nonmediated connection handles API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 15:59:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/717" class=".btn">#717</a>
            </td>
            <td>
                <b>
                    Nonmediated connection (de)serialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">feature</span>
            </td>
            <td>
                Exposes (de)serialization methods on nonmediated connection handler.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 11:42:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/716" class=".btn">#716</a>
            </td>
            <td>
                <b>
                    Tweak u32 handle releasing handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Came up as desired change while working on https://github.com/hyperledger/aries-vcx/pull/665

- Change behaviour of releasing to be more forgiving - in tests of `vcx-napi-rs` where we frequently initialize and deinitialize happens often, it happens that garbage collector calls `release` on handle which we have freed manually via `shutdown` function
- Additionally: move some tests from `api_c` to `api_vcx`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 21:28:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/715" class=".btn">#715</a>
            </td>
            <td>
                <b>
                    Remove public agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span><span class="chip">wrappers</span><span class="chip">breaking</span><span class="chip">agents</span>
            </td>
            <td>
                Removes any and all usage of public agents in the codebase. In Rust integration tests where connection bootstrapping was previously performed via a public agent, an alternative approach was temporarily (i.e. until mediated connection is removed) chosen: the connection request message is sent / received via a channel instead of a DidComm endpoint to avoid overhead associated with managing an open TCP socket per test in Rust. However, vcx-agent-core integration tests do exchange connection requests via DidComm endpoint.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 16:37:39 +0000 UTC
    </div>
</div>

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
- renamed `create_proof` -> `create_with_proof_request`, `create_proof_with_msgid`  -> `create_with_msgid`
- fix clippy warnings, `agency_update_agent_webhook` - > `update_webhook_url`
- pulled logic from `api_c` layer `vcx_connection_sign_data`, `vcx_connection_verify_signature `, `vcx_get_service_from_ledger `,  to `api_vcx`  layer
- remove unnecessary `await`s
- moved declaration of `VERSION_STRING` in `api_vcx` layer
- Removed unnecessary logs



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

