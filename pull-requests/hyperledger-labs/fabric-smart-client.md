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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/619" class=".btn">#619</a>
            </td>
            <td>
                <b>
                    Remove race conditions and simplify endpoint service constructor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes a few race conditions and simplifies the constructor for the endpoint service.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-08 09:31:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/618" class=".btn">#618</a>
            </td>
            <td>
                <b>
                    Fix data race errors 
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
        Created At 2024-07-06 19:32:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/617" class=".btn">#617</a>
            </td>
            <td>
                <b>
                    Remove usages of SP
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
        Created At 2024-07-05 09:45:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/616" class=".btn">#616</a>
            </td>
            <td>
                <b>
                    Unit tests for SDK wiring
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
        Created At 2024-07-05 07:36:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/615" class=".btn">#615</a>
            </td>
            <td>
                <b>
                    Remove static drivers for DB
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
        Created At 2024-07-04 21:09:23 +0000 UTC
    </div>
</div>

