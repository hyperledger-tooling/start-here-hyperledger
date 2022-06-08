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
                PR <a href="https://github.com/hyperledger/fabric/pull/3463" class=".btn">#3463</a>
            </td>
            <td>
                <b>
                    Document GetStateByRangeWithPagination behavior
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Document GetStateByRangeWithPagination behavior including
the difference between leveldb and couchdb that was identified in #3229.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 23:04:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3462" class=".btn">#3462</a>
            </td>
            <td>
                <b>
                    Fixed Found Typos (Backport #2939)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of PR #2939
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-05 17:39:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3461" class=".btn">#3461</a>
            </td>
            <td>
                <b>
                    Gateway support for chaincode event checkpointing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of c55b7eed46da67098f9393dbb23df4167a53ebff and 2f2e5aa3f9858928003969282a0b56b271e3ec9c from main branch.

Gateway service will use an `AfterTransactionId` field in a ChaincodeEventsRequest message to locate the exact chaincode event from which eventing should be resumed. Provides server-side support for client checkpointing of chaincode events in Fabric Gateway client API v1.1.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 17:35:43 +0000 UTC
    </div>
</div>

