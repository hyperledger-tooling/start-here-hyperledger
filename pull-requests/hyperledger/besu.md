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
                PR <a href="https://github.com/hyperledger/besu/pull/3544" class=".btn">#3544</a>
            </td>
            <td>
                <b>
                    Always show privacyGroupId on PrivateTransactionReceipt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - This is to provide a clearer way of knowing which `privacyGroupId` a private transaction ended up in.

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 11:12:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3543" class=".btn">#3543</a>
            </td>
            <td>
                <b>
                    Signed-off-by: Bhaskar Ram <bhaskar@parrtosec.in>
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgrade TLS version to 1.3 in BesuCommand.java
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 05:11:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3539" class=".btn">#3539</a>
            </td>
            <td>
                <b>
                    Trace APIs: add revert reason
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add revertReason to trace_transaction, trace_call, trace_callMany, trace_rawTransaction and trace_get

Note revertReason manually added to the relevant test files generated from OE.
Also added a new test file for trace_transaction.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 05:37:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3538" class=".btn">#3538</a>
            </td>
            <td>
                <b>
                    Updated netty
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Updated dependencies
* netty
* solidity plugin
* artifactory plugin
* jmh
* spring crypto
* testcontainers

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 00:26:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3536" class=".btn">#3536</a>
            </td>
            <td>
                <b>
                    Refactor graphqlcontext since getContext() is deprecated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sandra Wang <yx97.wang@gmail.com>

## PR description
This PR is focused on resolving the deprecated dependency of graphQL context.

Deprecated: `graphql.schema.DataFetchingEnvironment#getContext`

## Fixed Issue(s)
Issue #2776
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 00:04:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3535" class=".btn">#3535</a>
            </td>
            <td>
                <b>
                    [MINOR] quorum ATs use docker executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Use docker executor and jdk image as before (but keep medium resource class)

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-07 23:41:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3533" class=".btn">#3533</a>
            </td>
            <td>
                <b>
                    Acceptance test for execution engine apis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

Adds acceptance tests for the execution engine APIs

## Fixed Issue(s)
fixes #3484

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-07 15:41:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3532" class=".btn">#3532</a>
            </td>
            <td>
                <b>
                    Batching backward sync
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
 This PR is making changing backward sync to use the batching mechanism.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-07 14:13:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3531" class=".btn">#3531</a>
            </td>
            <td>
                <b>
                    add trace_callMany to CHANGELOG
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-07 09:01:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3530" class=".btn">#3530</a>
            </td>
            <td>
                <b>
                    upgrade vertx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Update vertx to 4.2.5

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-07 04:45:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3529" class=".btn">#3529</a>
            </td>
            <td>
                <b>
                    Updated dependencies including log4j
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                * log4j
* jackson databind
* guava
* dagger

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-07 03:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3525" class=".btn">#3525</a>
            </td>
            <td>
                <b>
                    Log initial sync stats every 10 secs at max to avoid spamming logs 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3450
## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 17:08:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3523" class=".btn">#3523</a>
            </td>
            <td>
                <b>
                    updated several dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Updated some but not all dependencies. 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 06:06:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3520" class=".btn">#3520</a>
            </td>
            <td>
                <b>
                    [MINOR] addressed some sonar code smells
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Fixed 4 code smells introduced recently to make sonar happy.
Also minor change to shorten help message for --X-alg-native-enabled CLI options

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 04:15:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3518" class=".btn">#3518</a>
            </td>
            <td>
                <b>
                    debug_accountAt - fixed issue with contract code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If contract address supplied as the account parameter to `debug_accountAt`, I get an Internal Error with this IllegalArgumentException:
```
Expected at most 32 bytes but got 44
java.lang.IllegalArgumentException: Expected at most 32 bytes but got 168
	at com.google.common.base.Preconditions.checkArgument(Preconditions.java:299)
	at org.apache.tuweni.bytes.Bytes32.leftPad(Bytes32.java:176)
	at org.hyperledger.besu.ethereum.api.jsonrpc.internal.results.Quantity.create(Quantity.java:54)
	at org.hyperledger.besu.ethereum.api.jsonrpc.internal.results.Quantity.create(Quantity.java:50)
	at org.hyperledger.besu.ethereum.api.jsonrpc.internal.methods.DebugAccountAt.debugAccountAtResult(DebugAccountAt.java:130)
	at org.hyperledger.besu.ethereum.api.jsonrpc.internal.methods.DebugAccountAtTest.testResult(DebugAccountAtTest.java:179)
	at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.base/java.lang.reflect.Method.invoke(Method.java:566)
	at org.junit.runners.model.FrameworkMethod$1.runReflectiveCall(FrameworkMethod.java:59)
	at org.junit.internal.runners.model.ReflectiveCallable.run(ReflectiveCallable.java:12)
	at org.junit.runners.model.FrameworkMethod.invokeExplosively(FrameworkMethod.java:56)
	at org.junit.internal.runners.statements.InvokeMethod.evaluate(InvokeMethod.java:17)
	at org.mockito.internal.runners.DefaultInternalRunner$1$1.evaluate(DefaultInternalRunner.java:55)
	at org.junit.runners.ParentRunner$3.evaluate(ParentRunner.java:306)
	at org.junit.runners.BlockJUnit4ClassRunner$1.evaluate(BlockJUnit4ClassRunner.java:100)
	at org.junit.runners.ParentRunner.runLeaf(ParentRunner.java:366)
	at org.junit.runners.BlockJUnit4ClassRunner.runChild(BlockJUnit4ClassRunner.java:103)
	at org.junit.runners.BlockJUnit4ClassRunner.runChild(BlockJUnit4ClassRunner.java:63)
	at org.junit.runners.ParentRunner$4.run(ParentRunner.java:331)
	at org.junit.runners.ParentRunner$1.schedule(ParentRunner.java:79)
	at org.junit.runners.ParentRunner.runChildren(ParentRunner.java:329)
	at org.junit.runners.ParentRunner.access$100(ParentRunner.java:66)
	at org.junit.runners.ParentRunner$2.evaluate(ParentRunner.java:293)
	at org.junit.runners.ParentRunner$3.evaluate(ParentRunner.java:306)
	at org.junit.runners.ParentRunner.run(ParentRunner.java:413)
	at org.mockito.internal.runners.DefaultInternalRunner$1.run(DefaultInternalRunner.java:100)
	at org.mockito.internal.runners.DefaultInternalRunner.run(DefaultInternalRunner.java:107)
	at org.mockito.internal.runners.StrictRunner.run(StrictRunner.java:41)
```
With this fix, I get this response
```
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": {
        "code": "0x608060405234801561001057600080fd5b506004361061002b5760003560e01c8063b27b880414610030575b600080fd5b61004a60048036038101906100459190610108565b61004c565b005b60606000806000604051935036600085376000803686885af490503d9150816000853e806000811461007d57610093565b60008311156100925761012085019350836040525b5b5060008114156100ec578473ffffffffffffffffffffffffffffffffffffffff167f410d96db3f80b0f89b36888c4d8a94004268f8d42309ac39b7bcba706293e099856040516100e3919061016e565b60405180910390a25b5050505050565b60008135905061010281610227565b92915050565b60006020828403121561011e5761011d610211565b5b600061012c848285016100f3565b91505092915050565b600061014082610190565b61014a818561019b565b935061015a8185602086016101de565b61016381610216565b840191505092915050565b600060208201905081810360008301526101888184610135565b905092915050565b600081519050919050565b600082825260208201905092915050565b60006101b7826101be565b9050919050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60005b838110156101fc5780820151818401526020810190506101e1565b8381111561020b576000848401525b50505050565b600080fd5b6000601f19601f8301169050919050565b610230816101ac565b811461023b57600080fd5b5056fea2646970667358221220fdfb5c371055342507b8fb9ca7b0c234f79819bd5cb05c0d467fb605de979eb564736f6c63430008060033",
        "nonce": "0x1",
        "balance": "0x0",
        "codehash": "0xf5f334d41776ed2828fc910d488a05c57fe7c2352aab2d16e30539d7726e1562"
    }
}
```

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 06:12:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3516" class=".btn">#3516</a>
            </td>
            <td>
                <b>
                    [MINOR] typo in resource class 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Address this error: Resource class "med" is not a valid resource class. The default resource class will be used. eg https://app.circleci.com/pipelines/github/hyperledger/besu/13609/workflows/3b159bdb-3556-4612-bb4f-3fa89c0271b4/jobs/76148
* And also fixed another typo

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 02:09:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3514" class=".btn">#3514</a>
            </td>
            <td>
                <b>
                    Emeritus 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I propose moving the following maintainer to Emeritus status, pursuant to the inactivity clause. These maintainers have had no activity since September 2021:
* @vmichalik  - last Besu activity was in September 2021 #2718 

We very much appreciate their contributions but moving their status to emeritus (and thus revoking PR approval privileges) is in the interest of an orderly project. If any of these maintainers express in this PR that they intend to make contributions in the next quarter, then they will not be moved to emeritus status.
I propose this vote is open until either an absolute majority of active maintainers votes for the same outcome, or until two weeks has passed, after which a voting majority will determine the outcome (with a tie resulting in no change).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 00:57:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3511" class=".btn">#3511</a>
            </td>
            <td>
                <b>
                    [#2766]fix: clean up deprecation warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sandra Wang <yx97.wang@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR is to clean up deprecation warnings raised in issue #2766 
This PR cleans up: 
- Quantity Interface getValue() [besu/plugin-api/src/main/java/org/hyperledger/besu/plugin/data/Quantity.java](https://github.com/hyperledger/besu/blob/35f16420eb5dc9e54a9510695316e8f590eee181/plugin-api/src/main/java/org/hyperledger/besu/plugin/data/Quantity.java#L35)
- OKHttpStreamClient
I am going to create more separate PRs to address warnings that are specific to the concerns. 

## Fixed Issue(s)
fixes #2766

I move `GraphQLDataFetcherContext` to a separate PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 21:42:10 +0000 UTC
    </div>
</div>

