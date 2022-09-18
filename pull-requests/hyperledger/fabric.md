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
                PR <a href="https://github.com/hyperledger/fabric/pull/3640" class=".btn">#3640</a>
            </td>
            <td>
                <b>
                    unit test flake in leadership transfer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
Bug fix

#### Description
When the leadership transfer not picked up the next leader, send out artificial MsgTimeOut msg to induce election.

#### Related issues
#3629 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-18 08:29:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3637" class=".btn">#3637</a>
            </td>
            <td>
                <b>
                    Ordrer v3: disable solo (WIP)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: I00846aa130d5b9fb486ace5f84898a0b0affddf5

- Improvement (improvement to code, performance, etc)

#### Description

- Disable the solo consenter in the orderer main
- fix unit tests that fail
- fix integration tests that fail

#### Related issues

Issue: #3514 
Epic: #3511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 06:55:22 +0000 UTC
    </div>
</div>

