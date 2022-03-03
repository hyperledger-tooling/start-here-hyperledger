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

## Fixed Issue(s)
fixes #2766

Hi reviewers, this is my first PR as a contributor. It is still WIP. Just want to get some opinion first to make sure I am on the right track. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 21:42:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3510" class=".btn">#3510</a>
            </td>
            <td>
                <b>
                    Refactor trace api methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Refactor trace api methods to pave way for 
https://github.com/hyperledger/besu/pull/3459
https://github.com/hyperledger/besu/pull/3477
https://github.com/hyperledger/besu/pull/3468

Two abstract classes for code reuse and minimise the amount of merge conflict needed fixing

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 04:21:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3508" class=".btn">#3508</a>
            </td>
            <td>
                <b>
                    3465 jwt auth
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
If merge and jwt auth is enabled, starts the Engine API (both websockets and http) requiring JWT auth as described in Kiln2 spec.

Extracts an AuthenticationService interface and provides a Default (legacy) implementation alongside an Engine specific implementation. Either may be used from HTTP or Websocket stacks.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3465 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 22:27:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3505" class=".btn">#3505</a>
            </td>
            <td>
                <b>
                    [Issue 3115] Support mining beneficiary transitions
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
Add the ability to transition the `miningbeneficiary` for *bft (ibft2, qbft) consensus mechanisms. 

Example genesis file with `miningbeneficiary` transitions:
```
{
  "config": {
    "chainId": 999,
    "byzantiumBlock": 0,
    "ibft2": {
      "blockperiodseconds": 1,
      "epochlength": 30000,
      "requesttimeoutseconds": 5,
      "blockreward": "5000000000000000000",
      "miningbeneficiary": "0x0000000000000000000000000000000000000001"
    },
    "transitions": {
      "ibft2": [
          {
              "block": 10000, 
              "miningbeneficiary": "",
          },
          {
              "block": 20000, 
              "miningbeneficiary": "0x0000000000000000000000000000000000000002",
          }
      ]
    }
  },
  ...
}
```
The `miningbeneficiary` will only be updated if there is a "miningbeneficiary" key in the `transitions.ibft2` array element.  Setting the `miningbeneficiary` to an empty value will clear out any override so that block rewards go to the miner rather than a global override address.  

Other changes:
* Keep the miningbeneficiary as an `Address` rather than a `String` in `BftConfigOptions` and make the conversion from `String` to `Address` strict (i.e. all 20 address bytes are required "0x01" is not valid). 
* Fix `ThreadBesuNodeRunner` so that it respects a node's genesis config.


## Fixed Issue(s)
Fixes #3115

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 17:05:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3503" class=".btn">#3503</a>
            </td>
            <td>
                <b>
                    Add GitHub action to verify gradle-wrapper.jar
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Checks that the gradle wrapper jar is from an official release since a maliciously modified jar added as part of a gradle upgrade would be a significant security risk but is hard to verify from the code diff.  This checks the jar comes from an Official Gradle release.

See https://github.com/gradle/wrapper-validation-action for more details.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 04:42:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3502" class=".btn">#3502</a>
            </td>
            <td>
                <b>
                    Update ef bootnodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Updates ef bootnode addresses
Geth PR: https://github.com/ethereum/go-ethereum/pull/24432

## Fixed Issue(s)
fixes #3488 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 02:28:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3501" class=".btn">#3501</a>
            </td>
            <td>
                <b>
                    Bugfix/terminal block check
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
Ensure besu correctly checks for latest ancestor before checking if a block descends from terminal.  

Also, forkchoiceUpdated calls for finalized blocks which besu does not have should start or append to a backward sync.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3500

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 23:32:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3499" class=".btn">#3499</a>
            </td>
            <td>
                <b>
                    Improve contract validation errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

For each contract validation error return a relevant error instead of
the incorrect "INSUFFICIENT_GAS" error.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 17:02:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3497" class=".btn">#3497</a>
            </td>
            <td>
                <b>
                    Prepare for release 22.1.2 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Prepare for release 22.1.2

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-25 00:44:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3496" class=".btn">#3496</a>
            </td>
            <td>
                <b>
                    Release 22.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Release 22.1.1

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 18:55:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3495" class=".btn">#3495</a>
            </td>
            <td>
                <b>
                    Rename field random to prevRandao
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

Renames the field `random` in ExecutionPayloadV1, PayloadAttributesV1 and the block header to `prevRandao` to be Kiln spec v2 compatible.

## PR description

## Fixed Issue(s)
fixes #3490

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 14:04:34 +0000 UTC
    </div>
</div>

