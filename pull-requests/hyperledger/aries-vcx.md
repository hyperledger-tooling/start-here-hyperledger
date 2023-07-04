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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/891" class=".btn">#891</a>
            </td>
            <td>
                <b>
                    Partially #870 - Simple Message Relay for testing/demo purposes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                TODO
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 11:08:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/890" class=".btn">#890</a>
            </td>
            <td>
                <b>
                    Enable compiling the workspace with --tests --all-features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span>
            </td>
            <td>
                A hotfix to enable compiling the workspace with `--tests --all-features`.

It is [recommended](https://doc.rust-lang.org/cargo/reference/features.html#feature-unification) that

> [...] features should be additive. That is, enabling a feature should not disable functionality, and it should usually be safe to enable any combination of features. [...]

meaning the code should compile with all features enabled as well.

(Selfish reason is that I am using these cargo options in the rust-analyzer settings globally to enable code completion and error / warnings hints in any Rust project in all code, including code compiled conditionally using features and all tests. If the workspace stops compiling before it reaches the code I am working on, I get no error hints.)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-30 07:10:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/889" class=".btn">#889</a>
            </td>
            <td>
                <b>
                    NodeJS wrapper with modular libs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ios</span><span class="chip">skip-android</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 17:39:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/888" class=".btn">#888</a>
            </td>
            <td>
                <b>
                    ci: run libvcx tests with modular features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ios</span><span class="chip">skip-android</span>
            </td>
            <td>
                ### `libvcx_core`
- Modify global state handling and init related functions to enable running both with legacy vdrtools and credx/indy-vdr setup

### `aries-vcx`
- tweak indyvdr error mapping

### New cargo features in `libvcx_core`, `libvcx`, `vcx-napi-rs`
- Added features `anoncreds_vdrtools` `anoncreds_credx` to select anoncreds implementation 
- Added features `ledger_vdrtools`, `ledger_indyvdr` to select ledger client implementation

### CI
- Leave only 1 code coverage job which runs both integration and unit tests in `aries-vcx`. The coverage jobs runs with modular libs profile
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 16:32:40 +0000 UTC
    </div>
</div>

