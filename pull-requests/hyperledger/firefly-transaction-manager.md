---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/117" class=".btn">#117</a>
            </td>
            <td>
                <b>
                    Pass in action occurred time
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly-transaction-manager/issues/111

Allow action occurred time to be passed in so the recorded time reflects the time when an action occurred.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-26 08:32:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/116" class=".btn">#116</a>
            </td>
            <td>
                <b>
                    fix: race condition when reading and writing to inflight queue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The policy loop frequently read and writes from the inflight queue, more specifically:
- It will load new transactions into the queue when it has space in `updateInFlightSet` and remove the ones that have completed.
- Remove transactions from the queue when it gets enough confirmations for that transaction

When loading new transactions, the code will take a copy and override the inflight queue with an empty array. If another thread was reading from such array, most often iterating to find a specific inflight tx it wouldn't find it.

This PR alongside with adding extra logging to help diagnose this sort of issues, adds a read/write mutex for the inflight queue and a mutex for each pendingState to be thread safe. Creates read locks when iterating and reading from the queue, write lock in a single place where we remove or load new transactions in queue and a mutex on the pendingState when we read or modify it.


Draft: as running another performance test for the latest commit
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 11:01:06 +0000 UTC
    </div>
</div>

