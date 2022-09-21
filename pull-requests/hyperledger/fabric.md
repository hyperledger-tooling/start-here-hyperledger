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
                PR <a href="https://github.com/hyperledger/fabric/pull/3642" class=".btn">#3642</a>
            </td>
            <td>
                <b>
                    verify leadership transfer status before waiting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix

#### Description
The thread which was waiting on the notifyc channel was not notified as the other thread well passed the execution before the channel gets established/initialized. Its a race condition between these 2 threads lead to the test case failure. Added additional check to check the status before waiting for notification from other go routine.

#### Related issues
#3629 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-20 19:02:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3641" class=".btn">#3641</a>
            </td>
            <td>
                <b>
                    Ordrer v3: stop using solo in orderer/common/server unit tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: I00846aa130d5b9fb486ace5f84898a0b0affddf5

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Stop using solo in orderer/common/server unit tests

#### Related issues

Issue: #3514 
Epic: #3511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-20 12:01:56 +0000 UTC
    </div>
</div>

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

