---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1208" class=".btn">#1208</a>
            </td>
            <td>
                <b>
                    Replace "UpsertBatch" with "InsertOrGetBatch"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                When persisting an off-chain batch initially received from data exchange or shared storage, it should always be an insert. If the batch exists, just move on. Otherwise we may accidentally revert a confirmed batch to its previous state if it happens to get redelivered.

Bonus: In addition to preventing bugs, this should give a tiny performance boost due to the optimistic batch insert.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 18:03:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1205" class=".btn">#1205</a>
            </td>
            <td>
                <b>
                    v1.1 backport: Re-poll immediately on full batch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #1204 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 05:16:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1204" class=".btn">#1204</a>
            </td>
            <td>
                <b>
                    Re-poll immediately on full batch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                After a rewind to recover from an missed batch (an occurrence of https://github.com/hyperledger/firefly-evmconnect/issues/53) I observed a slow recovery, and the logs seemed to show the Event Aggregator pausing for long periods rather than screaming through all the messages.

Investigating the code, I did not find anything that would prevent it waiting the full time in the case of having read a full page of events. This would mean when paging through old events a long way before the head, it could be very slow to recover.

> Note, you only notice this when in recovery mode after a rewind when events are not arriving frequently - as in that case there are no shoulder taps to naturally wake the event loop.
>
> Also, you only notice this when there is more than a full page (200) inflight pins to resolve, such that the aggregator has to keep spinning through those pages.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 05:13:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1203" class=".btn">#1203</a>
            </td>
            <td>
                <b>
                    [tokens] Only Use broadcastName for Multi-Party Namespaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We saw if `broadcastName` was set on a tokens plugin, token pools would fail to create within gateway namespaces:
```
[2023-03-01T20:25:10.568Z] ERROR Failed to activate token pool 'f2de67bb-5adf-4b98-ac06-7d25a19805ad': FF10272: Unknown tokens plugin 'erc20-erc721' ns=cok pid=1 role=event-manager
[2023-03-01T20:25:10.568Z] DEBUG fftokens updating operation cok:fb435cab-a2a5-4d1a-af28-f0bf84840c0b status=Failed error=FF10272: Unknown tokens plugin 'erc20-erc721' ns=cok pid=1
[2023-03-01T20:25:10.568Z] DEBUG SQL-> begin dbtx=N1fXw8pi ns=cok pid=1
[2023-03-01T20:25:10.568Z] DEBUG SQL<- begin dbtx=N1fXw8pi ns=cok pid=1
[2023-03-01T20:25:10.569Z] DEBUG SQL-> update operations dbtx=N1fXw8pi ns=cok pid=1
[2023-03-01T20:25:10.569Z] DEBUG SQL<- update operations affected=1 dbtx=N1fXw8pi ns=cok pid=1
[2023-03-01T20:25:10.569Z] DEBUG SQL-> lock cok dbtx=N1fXw8pi ns=cok pid=1
[2023-03-01T20:25:10.570Z] DEBUG SQL<- lock cok dbtx=N1fXw8pi ns=cok pid=1
[2023-03-01T20:25:10.570Z] DEBUG SQL-> insert events dbtx=N1fXw8pi ns=cok pid=1
[2023-03-01T20:25:10.570Z] DEBUG SQL<- insert events sequences=[9] dbtx=N1fXw8pi ns=cok pid=1
[2023-03-01T20:25:10.570Z] DEBUG SQL-> commit dbtx=N1fXw8pi ns=cok pid=1
[2023-03-01T20:25:10.573Z] DEBUG SQL<- commit dbtx=N1fXw8pi ns=cok pid=1
[2023-03-01T20:25:10.573Z]  INFO Emitted token_pool_op_failed event 47472d4f-70f7-4f3e-827d-a3e70c76cf72 for cok:fb435cab-a2a5-4d1a-af28-f0bf84840c0b (correlator=f2de67bb-5adf-4b98-ac06-7d25a19805ad,topic=f2de67bb-5adf-4b98-ac06-7d25a19805ad) dbtx=N1fXw8pi ns=cok pid=1
[2023-03-01T20:25:10.573Z]  INFO Inflight request 'f2de67bb-5adf-4b98-ac06-7d25a19805ad' resolved with timeout after 2068.43ms ns=cok pid=1 role=sync-async-bridge
[2023-03-01T20:25:10.573Z]  INFO <-- POST /api/v1/namespaces/cok/tokens/pools [400] (2071.90ms): FF10272: Unknown tokens plugin 'erc20-erc721' httpreq=hzG60xJW pid=1 req=Rd7exmVy
```

This is bc the definition handler doesn't know how to map the remote name back to the local name within gateway namespaces: https://github.com/hyperledger/firefly/blob/3b728534d50c0cee6ed27890114b5a4c44fcec5c/internal/definitions/handler_tokenpool.go#L36-L42

This fixes that by only using the `broadcastName` for multi-party namespaces when sending the token pool definition.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 04:27:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1202" class=".btn">#1202</a>
            </td>
            <td>
                <b>
                    Cleanup around batches and transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some general cleanup identified while working toward [FIR-17](https://github.com/hyperledger/firefly-fir/pull/17)

* Add helper FindOperationInTransaction
* Split internal batch dispatcher state from dispatched payload
* Add IsPinned() transaction helper
* Use message TransactionID in lookup
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 21:00:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1201" class=".btn">#1201</a>
            </td>
            <td>
                <b>
                    Run Solidity tests on GitHub PRs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 20:58:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1198" class=".btn">#1198</a>
            </td>
            <td>
                <b>
                    Fail gracefully when inserting many data rows on sqlite
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Need to pass requestConflictEmptyResult=true on this path, the same as we do on the postgres path.

Fixes #1196
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 19:12:46 +0000 UTC
    </div>
</div>

