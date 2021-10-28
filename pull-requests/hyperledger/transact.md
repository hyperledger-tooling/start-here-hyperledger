---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/238" class=".btn">#238</a>
            </td>
            <td>
                <b>
                    Stabilize protocol-sabre by moving to stable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 15:53:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/237" class=".btn">#237</a>
            </td>
            <td>
                <b>
                    `workload-runner` stabilization changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - make `DEFAULT_LOG_TIME_SECS` const private
- make `runner` module private
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 21:10:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/236" class=".btn">#236</a>
            </td>
            <td>
                <b>
                    Delete SqlMerkleState trees
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
        Created At 2021-10-27 16:18:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/235" class=".btn">#235</a>
            </td>
            <td>
                <b>
                    Drop experimental redis support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This feature is no longer of interest as it does not provide enough of the transactional guarantees required for its usage with merkle state.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 15:28:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/234" class=".btn">#234</a>
            </td>
            <td>
                <b>
                    Smallbank updates for stabilization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 15:05:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/233" class=".btn">#233</a>
            </td>
            <td>
                <b>
                    Replace expect with invalid transaction in command fam
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 14:02:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/232" class=".btn">#232</a>
            </td>
            <td>
                <b>
                    Stabilize sabre-compat by moving to wasm (stable)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 21:29:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/231" class=".btn">#231</a>
            </td>
            <td>
                <b>
                    Fixups for protocol-sabre feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rename protocol-sabre-exec to protocol-sabre and remove unused functions and variables from protocol::sabre.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 18:51:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/230" class=".btn">#230</a>
            </td>
            <td>
                <b>
                    Add sabre_command and sabre_smallbank to top-level Cargo.toml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes 'cargo clean' which in turn fixes 'just clean', and makes
sabre_command and sabre_smallbank use the shared target directory during
builds.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 16:51:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/229" class=".btn">#229</a>
            </td>
            <td>
                <b>
                    Update rust docs for sabre protocols
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 21:26:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/228" class=".btn">#228</a>
            </td>
            <td>
                <b>
                    Add release notes for 0.3.12
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
        Created At 2021-10-21 20:18:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/227" class=".btn">#227</a>
            </td>
            <td>
                <b>
                    sabre protocol doc typo fixes
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
        Created At 2021-10-21 19:33:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/226" class=".btn">#226</a>
            </td>
            <td>
                <b>
                    Fix typo in doc comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 19:25:33 +0000 UTC
    </div>
</div>

