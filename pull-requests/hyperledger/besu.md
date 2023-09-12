---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5865" class=".btn">#5865</a>
            </td>
            <td>
                <b>
                    Feature/multi version flat db [skip ci]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Draft version of multi-version flat db
* creates bonsai context concept
* extends FlatDbReaderStrategy to FlatDbStrategy, including writes
* creates FlatDbArchiveStrategy
* adds getNearestTo to SegmentedKeyValueStorage plugin-api  interface and implementations
* kikori worldstate provider integrated into BonsaiWorldStateProvider (not suitable for eth_getProof)

There are a handful of hacks that are marked with TODOs that are there for testing expedience.

skipping CI while in draft form

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5846 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 18:38:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5863" class=".btn">#5863</a>
            </td>
            <td>
                <b>
                    Merge MutableAccount and EVMAccount
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Merge MutableAccount and EVMAccount functionalities by removing EVMAccount, all calls to getMutable, and the WrappedEVMAccount that was wrapping non-EVMAccounts in a mutable fashion.  Instead, use a MutableAccount in all cases an EVMAccount would have been used.  This also tends to reduce a level of layering in many places.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-08 23:13:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5861" class=".btn">#5861</a>
            </td>
            <td>
                <b>
                    Don't start BFT mining coordinators until initial sync has completed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR is a suggested approach to resolving the NPE described in issue https://github.com/hyperledger/besu/issues/5856 whereby a QBFT block expiry timer causes a null pointer if the QBFT node is still syncing with the rest of the chain with `--sync-mode=FAST` or `--sync-mode=X_SNAP`

I have made the fix specific to BFT mining coordinators so that the behaviour of other consensus mining algorithms is unaffected by the change. I tested a lower-level fix to just for `null` in `TransactionPool.selectTransactions()` and that does indeed stop the NPE and allow the node to complete syncing successfully. However I have left the check out of this PR because it feels more appropriate to avoid any reason for trying to select transactions for a BFT miner that hasn't sync'd yet.

I've noted that while this prevents the NPE for `--sync-mode=X_SNAP` and the sync appears to complete successfully, the node does not participate in BFT block validation or proposals. I think that's a separate issue, and I assume it hasn't worked before since the NPE would have been hit. I suspect a new issue should be opened for that to be looked at separately but I'll wait for the conclusion of this PR.

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/5856
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-08 08:24:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5860" class=".btn">#5860</a>
            </td>
            <td>
                <b>
                    Move to Hyperledger large runners for current github actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Use the -8 and -16 large runners from HL org for the current github actions

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 20:02:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5859" class=".btn">#5859</a>
            </td>
            <td>
                <b>
                    docs(readme): fix broken link to installation of binaries page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #5858

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 00:00:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5857" class=".btn">#5857</a>
            </td>
            <td>
                <b>
                    Fix issue 5824 - Duplicate key errors in EthScheduler-Transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Fix Duplicate key errors in EthScheduler-Transactions like this one :
```
2023-08-29 19:31:22.624+00:00 | EthScheduler-Transactions-0 | ERROR | Besu | Uncaught exception in thread "EthScheduler-Transactions-0"
java.lang.IllegalStateException: Duplicate key 0xf526c3350c599fa381f0a9fd4412105d6e3b84cef407973520a4a536a602806d (attempted merging values ValidationResult{invalidReason=Optional.empty, errorMessage=Optional.empty} and ValidationResult{invalidReason=Optional[TRANSACTION_ALREADY_KNOWN], errorMessage=Optional.empty})
        at java.base/java.util.stream.Collectors.duplicateKeyException(Collectors.java:135)
        at java.base/java.util.stream.Collectors.lambda$uniqKeysMapAccumulator$1(Collectors.java:182)
        at java.base/java.util.stream.ReduceOps$3ReducingSink.accept(ReduceOps.java:169)
        at java.base/java.util.stream.SortedOps$SizedRefSortingSink.end(SortedOps.java:357)
        at java.base/java.util.stream.AbstractPipeline.copyInto(AbstractPipeline.java:510)
        at java.base/java.util.stream.AbstractPipeline.wrapAndCopyInto(AbstractPipeline.java:499)
        at java.base/java.util.stream.ReduceOps$ReduceOp.evaluateSequential(ReduceOps.java:921)
        at java.base/java.util.stream.AbstractPipeline.evaluate(AbstractPipeline.java:234)
        at java.base/java.util.stream.ReferencePipeline.collect(ReferencePipeline.java:682)
        at org.hyperledger.besu.ethereum.eth.transactions.TransactionPool.addRemoteTransactions(TransactionPool.java:212)
        at org.hyperledger.besu.ethereum.eth.transactions.TransactionsMessageProcessor.processTransactionsMessage(TransactionsMessageProcessor.java:87)
        at org.hyperledger.besu.ethereum.eth.transactions.TransactionsMessageProcessor.processTransactionsMessage(TransactionsMessageProcessor.java:60)
        at org.hyperledger.besu.ethereum.eth.transactions.TransactionsMessageHandler.lambda$exec$0(TransactionsMessageHandler.java:51)
        at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
        at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
        at java.base/java.lang.Thread.run(Thread.java:833)
```

**Unit Test without the modification in TransactionPool** 
<img width="1659" alt="image" src="https://github.com/hyperledger/besu/assets/5099602/e7ef3a8b-72d1-4e7d-a331-5d1baad2214b">

**Unit Test with the modification in TransactionPool** 
<img width="1659" alt="image" src="https://github.com/hyperledger/besu/assets/5099602/5c5c14bf-92fe-4986-b517-b02e8361de39">

## Fixed Issue(s)
#5824 
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 14:19:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5854" class=".btn">#5854</a>
            </td>
            <td>
                <b>
                    Bump version to 23.7.3-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 08:11:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5853" class=".btn">#5853</a>
            </td>
            <td>
                <b>
                    set the beacon root address to the correct value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
In EIP-4788 the address of the contract used to store and retrieve the parent beacon block roots has been changed. This PR sets the correct value.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 07:22:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5852" class=".btn">#5852</a>
            </td>
            <td>
                <b>
                    [MINOR] use non-deprecated authenticate methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refs (does not fix) #5851 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 04:11:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5847" class=".btn">#5847</a>
            </td>
            <td>
                <b>
                    Release 23.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Post burn-in release of 23.7.2

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 20:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5844" class=".btn">#5844</a>
            </td>
            <td>
                <b>
                    Range tracing with worldstate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Implement a method to trace a range of blocks and have access to the worldstate before and after the tracing

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 15:25:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5843" class=".btn">#5843</a>
            </td>
            <td>
                <b>
                    add parent beacon block root to payload id calculation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This fixes a problem where two engine_forkchoiceUpdated RPC calls with the same parameters, except for the parentBeaconBlockRoot, caused besu to produce a block with the wrong block hash.
The beacon root was not used in the calculation of the payload id, which meant that we were not updating the block production after the second call.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 08:10:50 +0000 UTC
    </div>
</div>

