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
                PR <a href="https://github.com/hyperledger/fabric/pull/2603" class=".btn">#2603</a>
            </td>
            <td>
                <b>
                    Fixed JIRA issue FLY2- 64
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I have updated chain.go  Submit and ordered method..

#Fixed FLY2-64
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 09:36:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2601" class=".btn">#2601</a>
            </td>
            <td>
                <b>
                    Maintain order of transactions in the commit notification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
Maintain order of transactions in the commit notification so the gateway can deliver the clients the chaincode events in the same and consistent order.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 18:21:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2599" class=".btn">#2599</a>
            </td>
            <td>
                <b>
                    FABGW-18: Fix concurrency issue in commit notifier close
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This code path should only be executed if the ledger notifications stop, which is never expected to happen at runtime. However, it does happen within the unit tests could cause an intermittent test failure.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 15:33:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2598" class=".btn">#2598</a>
            </td>
            <td>
                <b>
                    Bump vmImage to Ubuntu-20.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Just keeping up with latest deps

Signed-off-by: Brett Logan <lindluni@github.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 13:40:34 +0000 UTC
    </div>
</div>

