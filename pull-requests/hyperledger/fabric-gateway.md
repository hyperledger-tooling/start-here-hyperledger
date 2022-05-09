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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/432" class=".btn">#432</a>
            </td>
            <td>
                <b>
                    Use OptionalLong for Java checkpoint block number
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Block number will not be set in the initial checkpointer state, and
previously logic to detect this required that the block number be set to
zero and the transaction ID (which already uses an Optional) unset. This
can be simplified by using an Optional to indicate whether the block
number has a value.

Signed-off-by: Mark S. Lewis <Mark.S.Lewis@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-08 17:34:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/431" class=".btn">#431</a>
            </td>
            <td>
                <b>
                    Update Java dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes updates to isecurity vulnerability scanning and checkstyle.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 10:54:03 +0000 UTC
    </div>
</div>

