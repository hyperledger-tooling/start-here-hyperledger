---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/458" class=".btn">#458</a>
            </td>
            <td>
                <b>
                    Tidy-up Java dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 14:09:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/457" class=".btn">#457</a>
            </td>
            <td>
                <b>
                    Install Go tools as part of make targets that require them
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove explicit Go CLI command dependency install steps from Makefile and CI pipeline.
- Add explicit `go install` commands in make targets that require CLI commands.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 11:19:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/456" class=".btn">#456</a>
            </td>
            <td>
                <b>
                    Use fabric-protos package in Java client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                No longer need to download and compile protobuf stubs to be bundled directly into fabric-gateway package.

Closes #420
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 17:10:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/455" class=".btn">#455</a>
            </td>
            <td>
                <b>
                    Add make target to install required Go tools
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously this was coded into the Azure Pipelines build script, and also documented for manual set up in the README.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 16:50:58 +0000 UTC
    </div>
</div>

