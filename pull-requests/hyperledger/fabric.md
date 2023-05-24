---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4232" class=".btn">#4232</a>
            </td>
            <td>
                <b>
                    WIP: BFT: orderer can deliver header+sigs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                


Change-Id: I47e9767e7f322145291a8ffa498500ee99714cc6


#### Type of change

- New feature

#### Description
When the SeekInfo message SeekContentType is HEADER_WITH_SIGS, send a block with nil block.data.


#### Related issues


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-23 11:41:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4231" class=".btn">#4231</a>
            </td>
            <td>
                <b>
                    test that a join block does not define a system channel by verifying consortiums
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Test update

#### Description

Addition of an integration test to validate that when channel participation receives a join block, this block does not define a system channel

#### Related issues

issue: #4019 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 17:02:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4230" class=".btn">#4230</a>
            </td>
            <td>
                <b>
                    system channel cleanup - cleanup docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removal of system channel from docs.

#### Type of change

- Documentation update

#### Description

Removal of system channel from docs.

#### Related issues

Issue: #4211 .

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 10:31:40 +0000 UTC
    </div>
</div>

