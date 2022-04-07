---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/fabric/issues/3320" class=".btn">3320</a>
            </td>
            <td>
                <b>
                    Improve error message when deliver service is asked for a block that doesn't yet exist on the node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                Improve error message when deliver service is asked for a block that doesn't yet exist on the node.

This is all we get for now:
`[common.deliver] deliverBlocks -> ERRO 18d59 [channel: channel1] Error reading from channel, cause was: NOT_FOUND`

It is enough for Fabric developers to know what happened, but not for users or support personnel.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 03:50:36 +0000 UTC
    </div>
</div>

