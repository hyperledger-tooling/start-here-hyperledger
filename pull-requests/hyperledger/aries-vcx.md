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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1063" class=".btn">#1063</a>
            </td>
            <td>
                <b>
                    feat: support aries-askar
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
        Created At 2023-11-16 14:10:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1062" class=".btn">#1062</a>
            </td>
            <td>
                <b>
                    Increase timeout in nodejs test
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
        Created At 2023-11-15 22:31:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1061" class=".btn">#1061</a>
            </td>
            <td>
                <b>
                    refactor: Move agents to new root (aries) as per #1045
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
        Created At 2023-11-13 16:35:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1060" class=".btn">#1060</a>
            </td>
            <td>
                <b>
                    Cleanup logging dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Incrementally addressing https://github.com/hyperledger/aries-vcx/issues/1012 (considering file reorg PR)

Outstanding:
- `libvcx_logger` should not exists, each top level crate such as `libvcx_core`, `uniffi` or backchannel shall setup env logger (or other log macro implementations) themselves.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-12 22:56:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1059" class=".btn">#1059</a>
            </td>
            <td>
                <b>
                    Reorganize crates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                First incremental shot at https://github.com/hyperledger/aries-vcx/issues/1045

Trying to move what's not currently being worked on / shouldn't cause trouble. Moves:
- `aries-vcx-agent` under `aries/agents/rust`
- `agency_client`, `diddoc_legacy`, `libvcx_core`,  `libvdrtools` under `aries/legacy`
- `shared_vcx` under `aries/shared_vcx`
- node wrappers `node` and `vcx-napi-rs` under `aries/wrappers`
- `wallet_migrator` under `tools/`

And fixes paths wherever needed
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-12 22:48:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1058" class=".btn">#1058</a>
            </td>
            <td>
                <b>
                    Uniffi demo holder
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
        Created At 2023-11-11 19:23:07 +0000 UTC
    </div>
</div>

