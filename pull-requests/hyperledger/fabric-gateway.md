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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/438" class=".btn">#438</a>
            </td>
            <td>
                <b>
                    Per-call and default gRPC options in Java client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New API for specifying default gRPC call options that allows the use of the gRPC API to specify all options rather than providing a complete set of corresponding calls in the Fabric Gateway client API. The old API for setting default timeouts is still available, reimplemented using the new API, but is marked as deprecated.

Closes #289 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 12:24:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/437" class=".btn">#437</a>
            </td>
            <td>
                <b>
                    Allow per-call gRPC call options to be specified in Go client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contributes to #289
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 14:31:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/436" class=".btn">#436</a>
            </td>
            <td>
                <b>
                    Minor refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Change checkpointer.ts to checkpointer.d.ts since it contains only typings and no code. Avoid a spurious JavaScript module being generated and imported.
- Remove redundant async modifier on Elliptic Curve signing function.
- Change .eslintrc files from YAML to JavaScript to allow tsconfig directory to be correctly resolved. This removed the need for project subdirectories to be explicitly added to VS Code workspaces so they appear as a root directory in order to resolve the tsconfig correctly during linting.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 11:21:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/435" class=".btn">#435</a>
            </td>
            <td>
                <b>
                    Persist Proposal, Transaction, Commit and Event Objects (Node JS)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contributes to  #394 

Signed-off-by: sapthasurendran <saptha.surendran@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 11:16:14 +0000 UTC
    </div>
</div>

