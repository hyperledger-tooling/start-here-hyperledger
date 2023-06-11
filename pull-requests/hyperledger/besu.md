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
                PR <a href="https://github.com/hyperledger/besu/pull/5578" class=".btn">#5578</a>
            </td>
            <td>
                <b>
                    Migrate util from JUnit 4.0 to JUnit 5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrate util tests from JUnit 4.0 to JUnit 5.0
fixes: #5556 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-10 19:48:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5575" class=".btn">#5575</a>
            </td>
            <td>
                <b>
                    Migrate EVM module to JUnit 5
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

Migrate EVM module tests to JUnit 5.
Mostly parameterized test and mockito support changes.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-09 17:28:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5573" class=".btn">#5573</a>
            </td>
            <td>
                <b>
                    [MINOR] errorprone-checks - migrate to junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #5565 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-09 05:21:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5572" class=".btn">#5572</a>
            </td>
            <td>
                <b>
                    [MINOR] Datatypes - junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #5567 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-09 04:44:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5554" class=".btn">#5554</a>
            </td>
            <td>
                <b>
                    [4844] Add dataGasUsed and dataGasPrice to receipts for 4844 txs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
[4844] Add dataGasUsed and dataGasPrice to receipts for 4844 txs

## Fixed Issue(s)
#5489
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-09 03:30:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5552" class=".btn">#5552</a>
            </td>
            <td>
                <b>
                    fix spotless
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix spotless
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 18:18:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5551" class=".btn">#5551</a>
            </td>
            <td>
                <b>
                    Fix blob encoding/decoding for network issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix encoding/decoding issues with Blob Transactions for network

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 18:00:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5550" class=".btn">#5550</a>
            </td>
            <td>
                <b>
                    Renumber EOF and Transient storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

As per a recent ACD, the opcode numbers for EOF and Transient Storage have been updated.  Update the code and test cases for the new numbers.

Updated list https://hackmd.io/@shemnon/CancunOpcodeAllocation

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 14:43:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5548" class=".btn">#5548</a>
            </td>
            <td>
                <b>
                    Fix graphql storageAt for bonsai
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
This PR adds a check to the AccountAdapter used by the graphQL suite to ensure that if the account is a bonsaiAccount we open a new snapshot to retrieve the storage slot requested.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #5524
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 07:00:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5547" class=".btn">#5547</a>
            </td>
            <td>
                <b>
                    Make the return of hardforkfor optional
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Make the return of hardforkfor optional.

For the EngineGetPayloadV3, when Shanghai and Cancun had the same milestone, an exception was 

```
java.lang.IllegalStateException: No hardfork found for predicate org.hyperledger.besu.ethereum.api.jsonrpc.internal.methods.engine.EngineGetPayloadV3$$Lambda$840/0x00000008010a4838@237b2852
	at org.hyperledger.besu.ethereum.mainnet.DefaultProtocolSchedule.lambda$hardforkFor$4(DefaultProtocolSchedule.java:132)
	at java.base/java.util.Optional.orElseThrow(Optional.java:403)
	at org.hyperledger.besu.ethereum.mainnet.DefaultProtocolSchedule.hardforkFor(DefaultProtocolSchedule.java:131)
	at org.hyperledger.besu.consensus.merge.TransitionProtocolSchedule.lambda$hardforkFor$3(TransitionProtocolSchedule.java:210)
	at org.hyperledger.besu.consensus.merge.TransitionUtils.dispatchFunctionAccordingToMergeState(TransitionUtils.java:75)
	at org.hyperledger.besu.consensus.merge.TransitionProtocolSchedule.hardforkFor(TransitionProtocolSchedule.java:209)
	at org.hyperledger.besu.ethereum.api.jsonrpc.internal.methods.engine.EngineGetPayloadV3.<init>(EngineGetPayloadV3.java:55)
	at org.hyperledger.besu.ethereum.api.jsonrpc.methods.ExecutionEngineJsonRpcMethods.create(ExecutionEngineJsonRpcMethods.java:157)
	at org.hyperledger.besu.ethereum.api.jsonrpc.methods.ApiGroupJsonRpcMethods.create(ApiGroupJsonRpcMethods.java:30)
	at org.hyperledger.besu.ethereum.api.jsonrpc.methods.JsonRpcMethodsFactory.methods(JsonRpcMethodsFactory.java:144)
	at org.hyperledger.besu.RunnerBuilder.jsonRpcMethods(RunnerBuilder.java:1201)
	at org.hyperledger.besu.RunnerBuilder.build(RunnerBuilder.java:831)
	at org.hyperledger.besu.cli.BesuCommand.synchronize(BesuCommand.java:3086)
	at org.hyperledger.besu.cli.BesuCommand.buildRunner(BesuCommand.java:1725)
	at org.hyperledger.besu.cli.BesuCommand.run(BesuCommand.java:1560)
	at picocli.CommandLine.executeUserObject(CommandLine.java:2026)
	at picocli.CommandLine.access$1500(CommandLine.java:148)
	at picocli.CommandLine$RunLast.executeUserObjectOfLastSubcommandWithSameParent(CommandLine.java:2461)
	at picocli.CommandLine$RunLast.handle(CommandLine.java:2453)
	at picocli.CommandLine$RunLast.handle(CommandLine.java:2415)
	at picocli.CommandLine$AbstractParseResultHandler.execute(CommandLine.java:2273)
	at picocli.CommandLine$RunLast.execute(CommandLine.java:2417)
	at picocli.CommandLine.execute(CommandLine.java:2170)
	at org.hyperledger.besu.cli.util.ConfigOptionSearchAndRunHandler.handle(ConfigOptionSearchAndRunHandler.java:62)
	at org.hyperledger.besu.cli.util.ConfigOptionSearchAndRunHandler.handle(ConfigOptionSearchAndRunHandler.java:33)
	at picocli.CommandLine$AbstractParseResultHandler.execute(CommandLine.java:2273)
	at picocli.CommandLine$RunLast.execute(CommandLine.java:2417)
	at picocli.CommandLine.execute(CommandLine.java:2170)
	at org.hyperledger.besu.cli.BesuCommand.parse(BesuCommand.java:1717)
	at org.hyperledger.besu.cli.BesuCommand.parse(BesuCommand.java:1512)
	at org.hyperledger.besu.Besu.main(Besu.java:39)
```



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 06:07:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5546" class=".btn">#5546</a>
            </td>
            <td>
                <b>
                    validate versioned hashes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                compare versioned hashes passed in with those from blob tx
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 05:35:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5542" class=".btn">#5542</a>
            </td>
            <td>
                <b>
                    Improve log of p2p messages
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
For most p2p messages the `toString` was not implemented, and that made it harder to trace exchanged messages. This PR implements a base `toString` that prints the raw data, and if implemented in the sub class also the decoded format of the data.

Since message data could be quite large, the log system is configured to easily change the max amount of data written, according to the user needs, by default 1000 chars are written for raw data and decoded data.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-07 17:55:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5540" class=".btn">#5540</a>
            </td>
            <td>
                <b>
                    Remove deprecated Rinkeby network
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

Rinkeby has been [deprecated for removal](https://blog.ethereum.org/2022/06/21/testnet-deprecation) since last year and from June 1st it has been shutdown

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-07 12:31:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5538" class=".btn">#5538</a>
            </td>
            <td>
                <b>
                    remove PoW header validation if merge is enabled
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
Remove the Attached PoW rule used for the merge, as we are well past merge and this attached version of the PoW rule is causing unnecessary Ethash during chain sync:
![image](https://github.com/hyperledger/besu/assets/1238512/638f5c1f-e523-4ddb-a80a-10e4c3b6488e)


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
relates to #5539 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-06 15:57:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5537" class=".btn">#5537</a>
            </td>
            <td>
                <b>
                    Call operation performance optimizations 
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

- Introduce "undoable" journoled collections: set, map, table, and list
- Move values that are the same or shared across the transaction to
  TxValues record
- Move warm and cold storage to undoable sets and tables.
- Move transient storage to undoable table.
- Move address hashing inside of address with a memoized field.
- lazy create EOF return stack

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 18:04:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5536" class=".btn">#5536</a>
            </td>
            <td>
                <b>
                    EIP - 4844
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implements EIP-4844. 

- introduces a Hardfork class to the protocol schedule system
- new Engine APIs required for CL to work on 4844
- new DataGas type for tracking block cost for 4844 data
- new VersionedHash type to reflect that a versioned hash is not quite a pure sha256
- incorporates wrapped jc-kzg library for KZG point evaluations
- New transaction type, and domain objects for constituent parts to represent the Blobs, KZGCommitments, and Proofs used for 4844
- RLP encoders and decoders to support new transaction type
- gas pricing calculators for the new type of gas
- plugin-api version was changed

- TODO: KZGprecompile tests are failing, likely due to switch to big endian. Test is disabled, investigation ongoing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 14:57:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5534" class=".btn">#5534</a>
            </td>
            <td>
                <b>
                    Feature addition for tracing private transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Draft PR for adding priv_traceTransaction API

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5280
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 07:17:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5532" class=".btn">#5532</a>
            </td>
            <td>
                <b>
                    Remove push metrics port from effective ports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This results in a port conflict check however the push metrics port refers to a push gateway for besu to connect to rather than a port it is serving itself.

If you run besu with push metrics [following this guide](https://besu.hyperledger.org/en/stable/public-networks/how-to/monitor/metrics/#run-prometheus-with-besu-in-push-mode) then the bug fixed by this PR is that you have to run besu first, followed by the push gateway.

Now you can start either besu or push gateway in any order.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-04 20:54:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5531" class=".btn">#5531</a>
            </td>
            <td>
                <b>
                    Move ethstats server request to trace
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
        Created At 2023-06-04 20:43:43 +0000 UTC
    </div>
</div>

