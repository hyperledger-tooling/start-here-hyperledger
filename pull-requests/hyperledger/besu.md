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
                PR <a href="https://github.com/hyperledger/besu/pull/5305" class=".btn">#5305</a>
            </td>
            <td>
                <b>
                    Env var to debug child processes.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                export BESU_DEBUG_CHILD_PROCESS_PORT=5005 and when running ProcessBesuNodeRunner (i.e. acceptance tests) the child process will suspend and wait for a debugger to attach.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 15:33:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5303" class=".btn">#5303</a>
            </td>
            <td>
                <b>
                    [23.4] Remove GoQuorum privacy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Do not merge until the next release is 23.4
Fixes #4886

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 08:23:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5302" class=".btn">#5302</a>
            </td>
            <td>
                <b>
                    [23.4] Remove IBFT1 consensus mechanism
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This feature has been deprecated and is being removed in 23.4 (that is - do not merge until all other releases have been completed and 23.4 is the next release)

Fixes #4922 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 02:33:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5301" class=".btn">#5301</a>
            </td>
            <td>
                <b>
                    Ethstat retry fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Fix ethstats retry logic. Attempt to connect with and without ssl. If `--ethstats` is specified without a port, use port 443 (for wss://) and port 80 (for ws://) as defaults instead of 3000. This will help in k8 or similar environment where ethstats is running behind a reverse proxy.

Introduced optional `--ethstats-cacert-file`. This option specifies the path to the root CA (Certificate Authority) certificate file that has signed ethstats server certificate (or reverse proxy certificate). This option is optional. Useful in non-production setup.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4696 
Potentially #3792 

## Local Testing
https://github.com/usmansaleem/ethstats-proxy
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 01:07:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5295" class=".btn">#5295</a>
            </td>
            <td>
                <b>
                     EIP-6110: Add deposit validation and apis
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
Add deposit validation and related apis.
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#5004 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 04:47:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5294" class=".btn">#5294</a>
            </td>
            <td>
                <b>
                    BFT acceptance tests for Berlin and London
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
Add acceptance tests for IBFT2 and QBFT for the Berlin and London forks.

* Update the ibft and qbft genesis configs to use berlin as the default instead byzantium
* Add tests for Berlin fork with gas and without gas
* Add tests for London fork with gas and without gas including using Frontier and EIP-1559 transactions
* Changed the DSL to make it clearer when we are using EIP-1559 transactions
* Added support in DSL to do transfers with a gas price

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5282 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 03:51:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5292" class=".btn">#5292</a>
            </td>
            <td>
                <b>
                    Use cached header for latest eth_getBlockByNumber
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span>
            </td>
            <td>
                While syncing, it is possible that we access the cached header's number before the block itself has had chance to be imported. In other words there is a mismatch between cached blockNumber and non-cached blockHeader that is being retrieved for the RPC.

Discovered after adding debug in https://github.com/hyperledger/besu/pull/5288

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5281

## Testing

Tested X_SNAP with each CL on sepolia as well as nimbus on goerli.
Without the fix: prysm, lighthouse and nimbus received the error (see https://github.com/hyperledger/besu/issues/5281#issuecomment-1491753557).
With the fix: no errors
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-02 01:45:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5291" class=".btn">#5291</a>
            </td>
            <td>
                <b>
                    For PoS, use extraData that was configured in the mining-extra-data cli option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span>
            </td>
            <td>
                This was hardcoded to "0x" as part of The Merge implementation. 

Fixes https://github.com/hyperledger/besu/issues/4471
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-01 05:22:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5290" class=".btn">#5290</a>
            </td>
            <td>
                <b>
                    Layered Transaction Pool
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

This implements a new transaction pool (txpool for brevity), with the main goal to better manage nonce gaps, i.e. the possibility that the list of transactions that we see for a sender could not be in order neither contiguous, that could happen just of the way there are  broadcasted on the p2p network or intentionally to try to spam the txpool with non executable transactions (transactions that could not be included in a future block), so the goal is to try to keep in the pool transactions that could be selected for a future block proposal, and a the same time, without penalizing legitimate unordered transactions, that are only temporary non executable.

It is disabled by default, to enable use the option `Xlayered-tx-pool=true`

The main idea is to organize the txpool in an arbitrary number of layers, where each layer has specific rules and constraints that determine if a transaction belong or not to that layer and also the way transactions move across layers.

Some design choices that apply to all layers are that a transaction can only be in one layer at any time, and that layers are chained by priority, so the first layer has the transactions that are candidate for a block proposal, and the last layer basically is where transactions are dropped. Layers are meant to be added and removed in case of specific future needs.
When adding a new transaction, it is first tried on the first layer, if it is not accepted then the next one is tried and so on.
Layers could be limited by transaction number of by space, and when a layer if full, it overflow to the next one and so on, instead when some space is freed, usually when transactions are removed since confirmed in a block, transactions from the next layer are promoted until there is space.

The current implementation is based on 3 layers, plus the last one that just drop every transaction when the previous layers are full. The 3 layers are, in order:

1. Prioritized
2. Ready
3. Sparse

Prioritized: 
This is where candidate transactions are selected for creating a new block.
Transaction are ordered by the effective priority fee, and it is limited by size, 2000 by default, to reduce the overhead of the sorting and because that number is enough to fill any block, at the current gas limit.
Does not allow nonce gaps, and the first transaction for each sender must be the next one for that sender.
Eviction is done removing the transaction with the higher nonce for the sender of the less valuable transaction, to avoid creating nonce gaps, evicted transactions go into the next layer Ready.

Ready:
Similar to the Prioritized, it does not allow nonce gaps, and the first transaction for each sender must be the next one for that sender, but it is limited by space instead of count, thus allowing many more transactions, think about this layer like a buffer for the Prioritized.
Since it is meant to keep ten to hundred of thousand of transactions, it does not have a full ordering, like the previous, but only the first transaction for each sender is ordered using a stable value that is the max fee per gas.
Eviction is the same as the Prioritized, and evicted transaction go into the next layer Sparse.

Sparse:
This is the first layer where nonce gaps are allowed and where the first transaction for a sender could not be the next expected one for that sender.
The main purpose of this layer is to act as a purgatory for temporary unordered and/or non contiguous transactions, so that they could become ready asap the missing transactions arrive, or they are eventually evicted.
It also keep the less valuable ready transactions, that are evicted from the previous layer.
It is limited by space, and eviction select the oldest transaction first, that is sent to the End Layer that just drop it.
When promoting to the prev layer Ready, only transactions that will not create nonce gaps are selected, for that we need to keep track of the nonce distance for each sender. So we can say that is ordered by nonce distance for promotion.


I have run it on mainnet and compared it against the current implementation, using [mitmproxy](https://mitmproxy.org/) plus this [custom addon](https://gist.github.com/fab-10/d535b4d99e324b2564505d56e6a14c08) to simulate a block production every other FcU, and collected the result in this document [Layered Transaction Pool metrics.ods](https://github.com/hyperledger/besu/files/11137473/Layered.Transaction.Pool.metrics.ods), the results are good, and on average the Layered txpool produces with 12% more transactions in less time.


A bunch of new metrics have been added, that could be used to graph totals and details about each layer, like in this dashboard
![Screenshot 2023-04-03 at 13-08-29 Besu Full Layered TxPool - Besu - Dashboards - Grafana](https://user-images.githubusercontent.com/91944855/229492903-6c16b4de-1fa8-4e69-a137-cb487c6651d0.png)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 17:29:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5288" class=".btn">#5288</a>
            </td>
            <td>
                <b>
                    Log an error when RPC responds with INTERNAL_ERROR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span>
            </td>
            <td>
                I think this would impact all RPCs, except maybe engine API. I am interesting in eth_getBlockByNumber for debugging purposes.

Error looks like this:
```
Error processing method: eth_getBlockByNumber ["latest",false]
java.lang.NullPointerException: Cannot invoke \"org.hyperledger.besu.ethereum.core.BlockHeader.getHash()\" because \"headHeader\" is null
at org.hyperledger.besu.ethereum.api.jsonrpc.internal.methods.EthGetBlockByNumber.latestResult(EthGetBlockByNumber.java:86)
at org.hyperledger.besu.ethereum.api.jsonrpc.internal.methods.AbstractBlockParameterMethod.findResultByParamType(AbstractBlockParameterMethod.java:90)
at org.hyperledger.besu.ethereum.api.jsonrpc.internal.methods.AbstractBlockParameterMethod.response(AbstractBlockParameterMethod.java:102)
at org.hyperledger.besu.ethereum.api.jsonrpc.execution.BaseJsonRpcProcessor.process(BaseJsonRpcProcessor.java:44)
at org.hyperledger.besu.ethereum.api.jsonrpc.execution.TracedJsonRpcProcessor.process(TracedJsonRpcProcessor.java:41)
at org.hyperledger.besu.ethereum.api.jsonrpc.execution.TimedJsonRpcProcessor.process(TimedJsonRpcProcessor.java:45)
at org.hyperledger.besu.ethereum.api.jsonrpc.execution.AuthenticatedJsonRpcProcessor.process(AuthenticatedJsonRpcProcessor.java:51)
at org.hyperledger.besu.ethereum.api.jsonrpc.execution.JsonRpcExecutor.execute(JsonRpcExecutor.java:92)
at org.hyperledger.besu.ethereum.api.handlers.JsonRpcExecutorHandler.executeRequest(JsonRpcExecutorHandler.java:118)
at org.hyperledger.besu.ethereum.api.handlers.JsonRpcExecutorHandler.executeJsonObjectRequest(JsonRpcExecutorHandler.java:131)
at org.hyperledger.besu.ethereum.api.handlers.JsonRpcExecutorHandler.lambda$handler$0(JsonRpcExecutorHandler.java:78)
at io.vertx.ext.web.impl.BlockingHandlerDecorator.lambda$handle$0(BlockingHandlerDecorator.java:48)
at io.vertx.core.impl.ContextImpl.lambda$null$0(ContextImpl.java:159)
at io.vertx.core.impl.AbstractContext.dispatch(AbstractContext.java:100)
at io.vertx.core.impl.ContextImpl.lambda$executeBlocking$1(ContextImpl.java:157)
at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1136)
at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:635)
at io.netty.util.concurrent.FastThreadLocalRunnable.run(FastThreadLocalRunnable.java:30)
at java.base/java.lang.Thread.run(Thread.java:833)\n
```

Tested on sepolia for all CLs and nimbus on goerli
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 04:32:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5285" class=".btn">#5285</a>
            </td>
            <td>
                <b>
                    Reduce EVM module dependencies
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

Refactor crypto, datatypes, and plugin-api to reduce plugin APIs in the EVM.

Split crypto into crypto services and crypto algorithms
Reverse the dependency between datatyps and plugin-api.
Remove plugin Hash and Address types (use datatypes)
Move PublicKey and Quantity into datatypes.

Lots of changes to imports and build files, and some `fromPlugin` calls removed.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 18:53:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5284" class=".btn">#5284</a>
            </td>
            <td>
                <b>
                    [DRAFT] Insert missing nodes in the flat database
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
As part of this PR, we will be conducting tests on the previous PR #4546.
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 11:26:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5277" class=".btn">#5277</a>
            </td>
            <td>
                <b>
                    Make QBFT validator smart contract mode work with london fork
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should work when gas fees are used as well as for free gas networks

Override the transactionSimulator's default TransactionValidationParams with one that allows for exceeding the account balance (which effectively zeros the baseFee). This mimics the way that eth_estimateGas and eth_call are implemented.

Fixes https://github.com/hyperledger/besu/issues/5249
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 07:50:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5276" class=".btn">#5276</a>
            </td>
            <td>
                <b>
                    Fix BFT creating invalid blocks on London when zero base fee is used
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
This fixes an issue where on IBFT and QBFT invalid blocks are created by the proposer when using London with a zeroBaseFee.

The cause of this is that the ZeroBaseFeeMarket was returning true for the implementsDataFee check which meant that the excessDataGas field was added to the block header. This is only valid after Shanghai.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5270 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 06:37:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5275" class=".btn">#5275</a>
            </td>
            <td>
                <b>
                    [MINOR] Add log to show where we're reading the jwt from
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
Add a log to print the path where we loaded the engine jwt for better ux.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 00:02:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5274" class=".btn">#5274</a>
            </td>
            <td>
                <b>
                    continue despite test failures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I would like to propose some blasphemy:

we should run the weekly sonarqube job with gradle --continue so it proceeds on, regardless of test failure.

this week a flaky test failed, and so we got no analysis.
the sonarqube job produces no artifacts of any use, it is meant as a weekly diagnostic, so while blasphemous, I believe this to be safe.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 18:41:48 +0000 UTC
    </div>
</div>

