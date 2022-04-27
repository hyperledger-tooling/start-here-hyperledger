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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3759" class=".btn">#3759</a>
            </td>
            <td>
                <b>
                    Add errorprone to prevent Log4j direct usage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This pull request contains some leftovers from #3285 and, most importantly, adds an _error prone_ check for preventing Log4j usage.
Most of this commits were part of #3425 but they mostly abstract stuff from Log4j and are not Logback specific so I thought it would make sense to introduce them here as well.

Here is the full list of changes:
- [HEAD~6](https://github.com/diega/besu/commit/logging_tweaks~6): replace Log4j2 logger with Slf4j added since #3285
- [HEAD~5](https://github.com/diega/besu/commit/logging_tweaks~5): renames leftover method from #3285
- [HEAD~4](https://github.com/diega/besu/commit/logging_tweaks~4): removes Log4j2 usage dependencies relying on the `Log4j2ConfiguratorUtil` (this is for simplifying the last diff)
- [HEAD~3](https://github.com/diega/besu/commit/logging_tweaks~3): replace Log4j2 `ThreadContext` usage with Slf4j's `MDC`
- [HEAD~2](https://github.com/diega/besu/commit/logging_tweaks~2): this is to explicitly check allowed levels instead of depending on Log4j enum options
- [HEAD~1](https://github.com/diega/besu/commit/logging_tweaks~1): for the same reason than before, the level values are filtered by the received string 
- [HEAD](https://github.com/diega/besu/commit/logging_tweaks): adds error prone check for preventing `o.a.l.log4j.LogManager` usages

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 15:48:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3757" class=".btn">#3757</a>
            </td>
            <td>
                <b>
                    Proof of Stake banner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Makes the transition to proof of stake more apparent

Signed-off-by: Justin Florentine <justin+github@florentine.us>

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-24 23:20:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3755" class=".btn">#3755</a>
            </td>
            <td>
                <b>
                    Introduce RocksDbSegmentIdentifier to avoid changing the storege plug…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …in interface

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

A refactor of #3734 to avoid changing the storage plugin interface

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #3722 


## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-23 15:39:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3754" class=".btn">#3754</a>
            </td>
            <td>
                <b>
                    Improve snap logs
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

This PR will significantly improve the snapsync logs by adding more statistics
```
Snapsync in progress synced=17.66%, accounts=1757406, slots=17596376, codes=628631, nodes=26844745
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #3744
fixes #3742 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 15:26:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3753" class=".btn">#3753</a>
            </td>
            <td>
                <b>
                    GraalVM image - wrong folder permissions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matija Folnovic <mfolnovic@gmail.com>

## PR description

## Fixed Issue(s)
Fixes #3751 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 13:13:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3752" class=".btn">#3752</a>
            </td>
            <td>
                <b>
                    Web3J 4.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **ON HOLD**: waiting for `org.web3j:quorum` release (ref: [web3j-quorum#66](https://github.com/web3j/web3j-quorum/issues/66))

Update Web3J dependency

Signed-off-by: Diego López León <dieguitoll@gmail.com>

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 12:56:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3750" class=".btn">#3750</a>
            </td>
            <td>
                <b>
                    Ensure port clash is reported when engine-rpc-http-port clashes with default websocket port 8551
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/besu/issues/3721

Unit tests this will fail due to a known issue with MergeConfigOptions.setMergeEnabled
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 09:16:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3749" class=".btn">#3749</a>
            </td>
            <td>
                <b>
                    Rename SHA3 -> Keccak256
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ethereum doesn't do "offcial" sha3, we do keccak256.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

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

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 23:24:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3748" class=".btn">#3748</a>
            </td>
            <td>
                <b>
                    use paris evm config in merge protocolschedule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                catch exception on block persist so that it can be added to badBlocks

Signed-off-by: garyschulte <garyschulte@gmail.com>

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
        Created At 2022-04-21 18:09:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3747" class=".btn">#3747</a>
            </td>
            <td>
                <b>
                    Treat the nonce as unsigned long
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

We have to use a 64 bit value for nonce in order to be compliant with the Ethereum specifiaction. Currently we use `long` which is 64 bit, but normally only 63 bit are used for the value and one bit is used to indicate if the number is positive or negative. Which means that our nonce currently is only 63 bit long.

There are alternative functions that allow to treat `long` as a 64 bit unsigned integer, by simply interpreting all of the 64 bits as value. This PR intends to do that in order to avoid creating instances of classes like `UInt64` whenever we operate with the nonce.

## Fixed Issue(s)
Example: fixes #3702 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 06:59:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3745" class=".btn">#3745</a>
            </td>
            <td>
                <b>
                    Log full peers list on connect/disconnect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Log full list of Rlpx Connections and EthPeers (at TRACE level) on peer connect/disconnect (also added rudimentary "score" to PeerReputation - not used anywhere as yet) eg
```
2022-04-21 12:21:27.470+10:00 | pool-8-thread-1 | TRACE | RlpxAgent | 2 ConnectionsById {
LocallyInitiatedRlpxConnection initiatedAt:1650507687470 to 0x3548c87b9920ff16aa4bdcf01c85f25117a29ae1574d759bad48cc9463d8e9f7c3c1d1e9fb0d28e73898951f90e02714abb770fd6d22e90371882a45658800e9 disconnected? false,
LocallyInitiatedRlpxConnection initiatedAt:1650507687469 to 0xdcb9390953aec5dde1d60dd556c36827053ca9adaefd1b03f531592fea43824bae2919743f620bb8a9b6c2b9a54439771d4f9a74d261b74af7a10c2dd9f13c97 disconnected? false} 
```
and ethPeers (different example - note 2 peers with same enode, one is "disconnected")
```
2022-04-21 11:17:23.192+10:00 | nioEventLoopGroup-3-2 | TRACE | EthProtocolManager | 2 EthPeers {
Peer 0xdcb9390953aec5dde1... PeerReputation 100, validated? true, disconnected? false, 
Peer 0xdcb9390953aec5dde1... PeerReputation 100, validated? true, disconnected? true} 
```
See #3665 

Also log peer reputation on disconnect See #3666 eg
```
2022-04-21 13:01:33.990+10:00 | nioEventLoopGroup-3-2 | TRACE | EthPeer | handleDisconnect - peer... 0x3548c87b9920ff16aa, PeerReputation 100 
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
        Created At 2022-04-21 01:37:58 +0000 UTC
    </div>
</div>

