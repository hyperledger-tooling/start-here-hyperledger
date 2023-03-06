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
                TODOs
- [ ] Unit tests
- [ ] Additional E2E test for using broadcastName for both multi-party and gateway namespaces
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1197" class=".btn">#1197</a>
            </td>
            <td>
                <b>
                    Call Features() getter to read DB provider features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Looking into https://github.com/hyperledger/firefly/issues/1199 (originally due to https://github.com/hyperledger/firefly/issues/1196) it appears that we are referencing the `SQLCommon.features` struct field expecting it to have the features of the DB provider, but with the refactoring that took place under https://github.com/hyperledger/firefly/pull/1110 the `SQLCommon.features` field is actually populated by the DB provider. That's because there's now also a `Database.features` struct field in `firefly-common` which is the one that's actually been populated.

In this PR I've removed the `SQLCommon.features` field and where we try to read from it today, used instead the new `Features()` getter that I've added under `firefly-common` PR https://github.com/hyperledger/firefly-common/pull/49

~~This PR will remain in draft until https://github.com/hyperledger/firefly-common/pull/49 is approved and we have a new release of `firefly-common` to pull in.~~ (firefly-common v1.2.3 now released and pulled in under the latest commit)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 15:23:58 +0000 UTC
    </div>
</div>

