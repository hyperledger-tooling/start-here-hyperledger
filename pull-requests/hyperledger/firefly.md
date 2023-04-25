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
                PR <a href="https://github.com/hyperledger/firefly/pull/1291" class=".btn">#1291</a>
            </td>
            <td>
                <b>
                    Use a more optimistic approach when inserting token transfer events, …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …assuming that they are new and can be inserted without conflict, then handle errors if not
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 15:43:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1290" class=".btn">#1290</a>
            </td>
            <td>
                <b>
                    feat: Upgrade to latest ffresty with mTLS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on:
- https://github.com/hyperledger/firefly-common/pull/65
- https://github.com/hyperledger/firefly/pull/1289

Once those are in I'll update this one
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 15:18:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1289" class=".btn">#1289</a>
            </td>
            <td>
                <b>
                    chore: remove deprecated config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                - Remove deprecated config for blockchain, tokens, factory, database, dex and shared storaged config
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 09:28:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1288" class=".btn">#1288</a>
            </td>
            <td>
                <b>
                    Fix 1287
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1287 

In PR chain with #1280 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 18:50:57 +0000 UTC
    </div>
</div>

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

