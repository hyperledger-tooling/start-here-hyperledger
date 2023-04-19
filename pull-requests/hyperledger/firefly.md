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
                PR <a href="https://github.com/hyperledger/firefly/pull/1286" class=".btn">#1286</a>
            </td>
            <td>
                <b>
                    chore(ci): switch to dedicated Firefly runners
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
        Created At 2023-04-19 00:27:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1285" class=".btn">#1285</a>
            </td>
            <td>
                <b>
                    Enable workflows for release branch
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
        Created At 2023-04-18 22:06:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1284" class=".btn">#1284</a>
            </td>
            <td>
                <b>
                    v1.2: Replace "UpsertBatch" with "InsertOrGetBatch"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When persisting an off-chain batch initially received from data exchange or shared storage, it should always be an insert. If the batch exists, just move on. Otherwise we may accidentally revert a confirmed batch to its previous state if it happens to get redelivered.

Backport of #1208, #1209, and #1204
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 19:49:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1283" class=".btn">#1283</a>
            </td>
            <td>
                <b>
                    v1.2: Fix postgres optimizations, fail gracefully when inserting many data rows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a backport of https://github.com/hyperledger/firefly/pull/1197 and https://github.com/hyperledger/firefly/pull/1198 for the 1.2.x release branch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 16:46:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1282" class=".btn">#1282</a>
            </td>
            <td>
                <b>
                    Accept private groupinit messages from any signing key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since we allow private messages to originate from an unregistered blockchain signing key,
we must also accept groupinit messages from the same (since the first private message
to a group will trigger group creation as a side-effect).

Fixes #1247
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 15:28:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1281" class=".btn">#1281</a>
            </td>
            <td>
                <b>
                    Address coverage gap, and issue with intent propagation found via it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In addressing all the coverage gaps I found in main (`internal/database`,`internal/events` and `internal/identity`) I found an issue with the new `ResolveQuerySigningKey` using the wrong intent on a default branch. The higher `sign` intent would have been used, rather than `query`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 12:49:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1280" class=".btn">#1280</a>
            </td>
            <td>
                <b>
                    Fix timing issue between Init and ConfigReload of Namespace Manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Event after #1242 checked in, @awrichar saw an instance of #1250 in this test run, with slightly different symptoms https://github.com/hyperledger/firefly/actions/runs/4728313082/jobs/8389728445

~These are a nightmare to diagnose, as Go tests do not log start/end of tests (unless in full debug mode) so a `goroutine` bleading past the end of the test boundary is hard to debug. But with some staring, I believe the problem is that some tests was only waiting _once_ at the end for the reload, and because of that there's the possibility for timing to happen such that the reload is detected before the first initialization has completed.~

~This proposed change adds a wait in the middle~

> See additional diagnosis below
> - locking update to ensure state propagation issue due to a lack of locking between goroutines.
> - unit test file writing change to rename in, rather than write in place

```
panic: 
assert: mock: The method has been called over 1 times.
	Either do one more Mock.On("NamespaceRestarted").Return(...), or remove extra call.
	This call was unexpected:
		NamespaceRestarted(string,time.Time)
		0: "ns1"
		1: time.Date(2023, time.April, 18, 3, 40, 40, 19021351, time.Local)
	at: [/home/runner/work/firefly/firefly/internal/namespace/plugin.go:89 /home/runner/work/firefly/firefly/internal/namespace/manager.go:314 /home/runner/work/firefly/firefly/internal/namespace/retry.go:56 /home/runner/work/firefly/firefly/internal/namespace/manager.go:301 /home/runner/work/firefly/firefly/internal/namespace/asm_amd64.s:1571]
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 12:31:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1279" class=".btn">#1279</a>
            </td>
            <td>
                <b>
                    Separate "define" and "publish" for contract interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                Part of the fix for #1220
In a chain with #1261
Depends on https://github.com/hyperledger/firefly-common/pull/64
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 03:40:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1278" class=".btn">#1278</a>
            </td>
            <td>
                <b>
                    Do not retry after a rejected message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes regression from #1251
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 03:27:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1275" class=".btn">#1275</a>
            </td>
            <td>
                <b>
                    Fix updating Contract APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly/issues/1274
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 17:15:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1273" class=".btn">#1273</a>
            </td>
            <td>
                <b>
                    Include signing key in batch processor identifier
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Messages from the same identity but different signing keys must be processed into different batches. If the signing key of the message does not match the signing key of the batch, the message will be rejected.

Backport of #1175 for 1.1.x
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 13:08:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1271" class=".btn">#1271</a>
            </td>
            <td>
                <b>
                    Pass `key` on queries to blockchain, after resolving with an intent to query
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently on a `query` to a custom blockchain transaction:
- FireFly resolves the `key` from the input, with an intent to `sign` a blockchain transaction (rather than do a query)
- Discards the `key` without passing it to EVMConnect/FabConnect

This is problematic in EVM based chains, where even you can simulate a transaction with `eth_call` from any signing address (without signing), and the result of the execution of that query might be different based on the input signing key.

So this PR proposes:
- Introducing a new `query` intent for resolving the key
- Passing the `signingKey` to the connector
- Updating Ethereum and Fabric implementations to pass this key to the connector

> Also includes a manifest change to pull in https://github.com/hyperledger/firefly-evmconnect/pull/74
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 00:04:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1269" class=".btn">#1269</a>
            </td>
            <td>
                <b>
                    Try out large runners to see if they are faster.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We are in a beta for large runners, and I want to see if this workflow is faster using them.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 15:28:02 +0000 UTC
    </div>
</div>

