---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/627" class=".btn">#627</a>
            </td>
            <td>
                <b>
                    Fixes for sessions
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
        Created At 2024-07-15 23:04:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/626" class=".btn">#626</a>
            </td>
            <td>
                <b>
                    Fixes
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
        Created At 2024-07-15 23:03:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/624" class=".btn">#624</a>
            </td>
            <td>
                <b>
                    Multiplex websockets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvement</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-12 22:09:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/622" class=".btn">#622</a>
            </td>
            <td>
                <b>
                    orion v0.2.10
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
        Created At 2024-07-10 13:09:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/621" class=".btn">#621</a>
            </td>
            <td>
                <b>
                    hide pkcs11 behind a build tag so that fsc is pure go by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `github.com/hyperledger/fabric/bccsp/pkcs11` dependency is the only reason we need CGO_ENABLED=1 when building an application that imports FSC. It makes things like cross-architecture builds unnecessarily difficult.

This PR makes it so that if you want to use pkcs11, you have to build the binary with `go build -tags pkcs11`. It includes a default implementation that panics if the user configures HSM in a binary that's not built with `pkcs11` as a build tag.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-09 14:57:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/620" class=".btn">#620</a>
            </td>
            <td>
                <b>
                    Added traces
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
        Created At 2024-07-09 10:58:06 +0000 UTC
    </div>
</div>

