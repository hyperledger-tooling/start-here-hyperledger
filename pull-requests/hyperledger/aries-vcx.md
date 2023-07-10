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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/896" class=".btn">#896</a>
            </td>
            <td>
                <b>
                    Initialize UniFFI demo and scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Initializes the base for building and testing uniffi demo application.
- Added convenience scripts for setting up and compiling uniffi_aries_vcx project for android.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 02:23:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/895" class=".btn">#895</a>
            </td>
            <td>
                <b>
                    Added capability of migrating wallet through the node.js wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Exposes the wallet migration functionality in the Node.js wrapper
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 11:53:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/894" class=".btn">#894</a>
            </td>
            <td>
                <b>
                    Update dependencies and AriesMessage Deserialize impl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #893.

Also updates `transitive` dependency and simplifies the `Deserialize` impl for `AriesMessage` to require less of `serde`'s internal components. 

Now only `Content` and `ContentDeserializer` are used merely at a type level, and these have been around for a very long time and are pretty much stable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 09:32:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/892" class=".btn">#892</a>
            </td>
            <td>
                <b>
                    libvcx implementation profiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ####  Note: the original PR https://github.com/hyperledger/aries-vcx/pull/888 got mis-merged into already merged branch, instead of being merged into `main`, hence I've recreated this PR with correct target branch

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
        Created At 2023-07-05 10:05:24 +0000 UTC
    </div>
</div>

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

