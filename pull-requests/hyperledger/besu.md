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
                PR <a href="https://github.com/hyperledger/besu/pull/3778" class=".btn">#3778</a>
            </td>
            <td>
                <b>
                    [DO NOT MERGE] Performance test : test Amazon ACCP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Test Amazon ACCP implementation
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 09:43:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3777" class=".btn">#3777</a>
            </td>
            <td>
                <b>
                    changed for loops with int vs long comparison
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Where int was being compared with long. Mostly int being used to iterate over values which could be long.
Not sure about these 2 since they are dealing with uint
- FlexiblePrivacyGroupContract
- FlexiblePrivacyGroupContract

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 06:43:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3776" class=".btn">#3776</a>
            </td>
            <td>
                <b>
                    Remove Leading Zeros from TransactionPendingResult
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                ## PR description

Currently, there is an issue with the way `TransactionPendingResult` gets serialized by in the JSON-RPC subsystem. Specifically, when responding to `eth_getTransactionByHash,` the `gasPrice`, `maxFeePerGas`, and `maxPriorityFeePerGas` values should be Quantities without leading zeros like so:

```
    "gas" : "0x11e63",
    "gasPrice" : "0x77359407",
    "maxPriorityFeePerGas" : "0x77359400",
    "maxFeePerGas" : "0xd09dc3000",
```

This is the official behavior defined in the spec and the behavior demonstrated by Geth and Nethermind.

However, in Besu, they are treated like 32-byte arrays and serialized with the leading zeros in place:

```
    "gas" : "0x10c83",
    "gasPrice" : "0x0000000000000000000000000000000000000000000000000000000ab5d04c00",
    "maxFeePerGas" : "0x0000000000000000000000000000000000000000000000000000000ab5d04c00",
```

This is a simple oversight caused by using `Wei.toHexString()` instead of `Wei.toShortHexString()`, which this PR addresses.

@frankisawesome has offered to fix the relevant unit tests that were unable to catch this, and will attach the fixes to this PR when they are ready.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 05:24:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3774" class=".btn">#3774</a>
            </td>
            <td>
                <b>
                    adding codeql to besu to check for quality
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
Adding codeql scans to HLF Besu


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 05:21:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3773" class=".btn">#3773</a>
            </td>
            <td>
                <b>
                    fix nullpointer on snapsync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Fixes a bug that caused Besu to not restart healing properly when changing pivot blocks. Snapsync thought the sync was done instead of restarting on a new pivot block. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 15:11:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3772" class=".btn">#3772</a>
            </td>
            <td>
                <b>
                    update version and changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 09:56:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3771" class=".btn">#3771</a>
            </td>
            <td>
                <b>
                    update version to 22.4.0-RC3-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 09:34:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3770" class=".btn">#3770</a>
            </td>
            <td>
                <b>
                    Release 22.4.0-RC2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.4.0-RC2
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 08:57:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3768" class=".btn">#3768</a>
            </td>
            <td>
                <b>
                    Set mainnet default gasLimit to 30M. Fixed #3767
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update default gasLimit in preparation for The Merge™. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 18:47:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3766" class=".btn">#3766</a>
            </td>
            <td>
                <b>
                    block import optimization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR makes significant changes during the block import (fast/snap sync) in order to speed up the synchronization time of Besu

This is the list of modification :
- A significant number of useless rlp `encode/decode` takes place during synchronization. Here is an example of useless encode/decode
    - Decode RLP from peer to have a Transaction object
    - After encode this transaction to rlp in order to calculate the hash of the transaction
    - Encode again this transaction to rlp in order to calculate the transactionRoot
    - Encode again this transaction to rlp in order to save the trx into the DB
    This is the same for all objects like `BlockHeader`, `BlockBody`, `Transaction`, `transactionReceipt`. The idea is to keep the rlp when decoding to use it if we need rlp again. 
- We do the generation of the `Receiptroot`, `transactionRoot` and `ommerHash` for the same block several times.
We do this at the time of the `GetBodiesFromPeerTask` and the `GetReceiptsFromPeerTask` but we also do it at the time of the `body validation`. So we calculate these values twice there.
The problem is that these are very consuming steps because we have to recreate a trie based on transactions and receipts. The idea is to store it in an optional field header and so if we already have it we don't need to calculate it again
- In the `GetBodiesFromPeerTask` and the `GetReceiptsFromPeerTask` methods we do the validations of the `Receiptroot` and the `transactionRoot` in parallel instead of doing it block by block. this saves time and like that we have all the root for the import part already calculated
- We also force the generation of the transaction Hash in parallel in the `GetBodiesFromPeerTask`. We need this hash during the import step in order to save the location of the each transaction hash in a block. It's better to calculate the hash in parallel during this step
- We validate the `block header` twice. During this step `CheckpointHeaderValidationStep` but also when calling the `fastImportBlock` method. Every time we want to validate a block we check a random to know if we want a full validation or not (1 chance out of 100 to make a full). The problem is even more important in POW because we have more chance for the same block to do a full check becaure we are calling two times this method `headerValidationPolicy.getValidationModeForNextBlock()`. So even more chance to do a full validation of a block on the mainnet
- Too many slow observers that impact the blocki import
  - TransactionPool (useless during block  import)
  - AbstractMiningCoordinator  (useless during block  import)
  - SyncState (useless during block  import)
  - FilterManager (useless during block  import)
  - LogSubscriptionService (useless during block  import)
  
  I keep :
   - NewBlockHeadersSubscriptionService
   - TransactionLogBloomCacher

  After we will have a fullsync with all observers


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 11:45:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3765" class=".btn">#3765</a>
            </td>
            <td>
                <b>
                    Node onchain permissioning startup validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fail besu startup if the node permissioning smart contract version check fails. This validation was not running because of the sync status check, which is more permissive until the node is in sync. At some point the "validate smart contract at startup" got hidden by the sync status check - so it wasn't even doing the smart contract check at that point.

With this change, if the version matches you will see this scroll on by in the logs
```
2022-04-27 11:35:53.845+10:00 | main | DEBUG | NodePermissioningControllerFactory | Validating onchain node permissioning smart contract configuration 
2022-04-27 11:35:53.888+10:00 | main | DEBUG | NodePermissioningControllerFactory | Successful validation of onchain node permissioning smart contract configuration! 
```
However if your smart contract does NOT match the version you specify, you get an error like this (admittedly a bit messy)
```
2022-04-27 11:34:21.170+10:00 | main | DEBUG | NodePermissioningControllerFactory | Validating onchain node permissioning smart contract configuration 
picocli.CommandLine$ParameterException: Error: node permissioning contract at address 0x0000000000000000000000000000000000009999 does not match the expected interface version 2.
	at org.hyperledger.besu.cli.BesuCommand.run(BesuCommand.java:1411)
	at picocli.CommandLine.executeUserObject(CommandLine.java:1939)
	at picocli.CommandLine.access$1300(CommandLine.java:145)
	at picocli.CommandLine$RunLast.executeUserObjectOfLastSubcommandWithSameParent(CommandLine.java:2358)
	at picocli.CommandLine$RunLast.handle(CommandLine.java:2352)
	at picocli.CommandLine$RunLast.handle(CommandLine.java:2314)
	at picocli.CommandLine$AbstractParseResultHandler.handleParseResult(CommandLine.java:2172)
	at picocli.CommandLine.parseWithHandlers(CommandLine.java:2559)
	at org.hyperledger.besu.cli.util.ConfigOptionSearchAndRunHandler.handle(ConfigOptionSearchAndRunHandler.java:54)
	at org.hyperledger.besu.cli.util.ConfigOptionSearchAndRunHandler.handle(ConfigOptionSearchAndRunHandler.java:31)
	at picocli.CommandLine$AbstractParseResultHandler.handleParseResult(CommandLine.java:2172)
	at picocli.CommandLine.parseWithHandlers(CommandLine.java:2559)
	at org.hyperledger.besu.cli.BesuCommand.parse(BesuCommand.java:1563)
	at org.hyperledger.besu.cli.BesuCommand.parse(BesuCommand.java:1371)
	at org.hyperledger.besu.Besu.main(Besu.java:49)
Caused by: java.lang.IllegalStateException: Error: node permissioning contract at address 0x0000000000000000000000000000000000009999 does not match the expected interface version 2.
	at org.hyperledger.besu.ethereum.permissioning.NodePermissioningControllerFactory.validatePermissioningContract(NodePermissioningControllerFactory.java:179)
	at org.hyperledger.besu.ethereum.permissioning.NodePermissioningControllerFactory.lambda$create$1(NodePermissioningControllerFactory.java:112)
	at java.base/java.util.Optional.ifPresent(Optional.java:183)
	at org.hyperledger.besu.ethereum.permissioning.NodePermissioningControllerFactory.create(NodePermissioningControllerFactory.java:109)
	at org.hyperledger.besu.RunnerBuilder.buildNodePermissioningController(RunnerBuilder.java:925)
	at org.hyperledger.besu.RunnerBuilder.build(RunnerBuilder.java:471)
	at org.hyperledger.besu.cli.BesuCommand.synchronize(BesuCommand.java:2825)
	at org.hyperledger.besu.cli.BesuCommand.buildRunner(BesuCommand.java:1572)
	at org.hyperledger.besu.cli.BesuCommand.run(BesuCommand.java:1400)
	... 14 more
Caused by: java.lang.IllegalStateException: Unable to check permissions for enode://6f8a80d14311c39f35f516fa664deaaaa13e85b2f7493f37f6144d86991ec012937307647bd3b9a82abe2974e1407241d54947bbb39763a4cac9f77166ad92a0@10.3.58.6:30303
	at org.hyperledger.besu.ethereum.permissioning.NodeSmartContractV2PermissioningController.isPermitted(NodeSmartContractV2PermissioningController.java:73)
	at org.hyperledger.besu.ethereum.permissioning.NodeSmartContractV2PermissioningController.checkSmartContractRules(NodeSmartContractV2PermissioningController.java:60)
	at org.hyperledger.besu.ethereum.permissioning.AbstractNodeSmartContractPermissioningController.isConnectionPermitted(AbstractNodeSmartContractPermissioningController.java:87)
	at org.hyperledger.besu.ethereum.permissioning.node.NodePermissioningController.isPermitted(NodePermissioningController.java:98)
	at org.hyperledger.besu.ethereum.permissioning.NodePermissioningControllerFactory.validatePermissioningContract(NodePermissioningControllerFactory.java:166)
	... 22 more
Caused by: java.lang.IllegalStateException: Failed node permissioning smart contract call
	at org.hyperledger.besu.ethereum.permissioning.NodeSmartContractV2PermissioningController.parseResult(NodeSmartContractV2PermissioningController.java:120)
	at java.base/java.util.Optional.map(Optional.java:265)
	at org.hyperledger.besu.ethereum.permissioning.NodeSmartContractV2PermissioningController.getCallResult(NodeSmartContractV2PermissioningController.java:82)
	at org.hyperledger.besu.ethereum.permissioning.NodeSmartContractV2PermissioningController.isPermitted(NodeSmartContractV2PermissioningController.java:65)
	... 26 more

To display full help:
besu [COMMAND] --help
Caused by: java.lang.IllegalStateException: Error: node permissioning contract at address 0x0000000000000000000000000000000000009999 does not match the expected interface version 2.

Caused by: java.lang.IllegalStateException: Unable to check permissions for enode://6f8a80d14311c39f35f516fa664deaaaa13e85b2f7493f37f6144d86991ec012937307647bd3b9a82abe2974e1407241d54947bbb39763a4cac9f77166ad92a0@10.3.58.6:30303

Caused by: java.lang.IllegalStateException: Failed node permissioning smart contract call


> Task :besu:Besu.main() FAILED

Execution failed for task ':besu:Besu.main()'.
```
## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 01:17:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3761" class=".btn">#3761</a>
            </td>
            <td>
                <b>
                    Fix heal stall issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR is a candidate fix for the healing that was stuck.
The problem only came when we had a pivot block change. In some cases we were creating new tasks with the old pivot block which could block the node in an endless cycle of request in error on a bad pivot block.

Tested on goerli (ok)
Mainnet test in progress


## Fixed Issue(s)
fixes https://github.com/hyperledger/besu/issues/3742


- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 08:53:37 +0000 UTC
    </div>
</div>

