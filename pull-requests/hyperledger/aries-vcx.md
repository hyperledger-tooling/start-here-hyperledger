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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/898" class=".btn">#898</a>
            </td>
            <td>
                <b>
                    Cleanup/constant
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
        Created At 2023-07-13 15:00:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/897" class=".btn">#897</a>
            </td>
            <td>
                <b>
                    Refactor dealing with tails_dir in tests
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
        Created At 2023-07-13 14:39:48 +0000 UTC
    </div>
</div>

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

