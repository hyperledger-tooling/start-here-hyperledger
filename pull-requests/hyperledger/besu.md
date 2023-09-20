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
                PR <a href="https://github.com/hyperledger/besu/pull/5909" class=".btn">#5909</a>
            </td>
            <td>
                <b>
                    Process onBlockAdded event asyncronously
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

Reduce `engine_forkchoiceUpdatedV?` response time by asynchronously process block added events in the transaction pool.
This way the processing of the block in the txpool will not add to the response time of the method, and according to my test the gain is evident (yellow line instance is running this PR)
![image](https://github.com/hyperledger/besu/assets/91944855/ce469f1d-3723-4dcd-8bc4-575f3c079f87)

The implementation makes sure that block events are processed sequentially in the order they arrive.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-20 09:10:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5906" class=".btn">#5906</a>
            </td>
            <td>
                <b>
                    Burn in candidate for 23.7.3
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
        Created At 2023-09-20 05:56:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5905" class=".btn">#5905</a>
            </td>
            <td>
                <b>
                    Burn in release of 23.7.3 from main (inclusive of sha eef40bd)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ---

Drop Kotti Network support (ETC) (#5816)



fix ForkId if there are no Forks and the starting timestamp is not 0 (#5819)



enforce that BlobTransactions have at least one blob (#5826)

* enforce that BlobTransactions have at least one blob




Do not create ignorable segments on `revert storage-variables` (#5830)

* fix the bug that creates the ignorable chain pruner segment, add rocks exception parsing to RocksDBColumnarKeyValueStorage subclasses
* parse rocksdb error for unprintable column family id's



add versioned hashes and number of blobs to toString() (#5831)



add parent beacon block root to payload id calculation (#5843)



bump version to 23.7.3-SNAPSHOT (#5854)



set the beacon root address to the correct value (#5853)



docs(readme): fix broken link to installation of binaries page (#5859)

Fixes #5858



Update RocksDB version from 8.0.0 to 8.3.2 (#5832)





use non-deprecated authenticate methods (#5852)



move to Hyperledger shared runners for current github actions (#5860)



Add range tracing with worldstate (#5844)

Implement a method to trace a range of blocks and have access to the worldstate before and after the tracing



Layered txpool by default and txpool options hoverhaul (#5772)



Fix issue 5824 - Duplicate key errors in EthScheduler-Transactions (#5857)

Fix issue 5824 - Duplicate key errors in EthScheduler-Transactions



updated gradle verification metadata (#5870)

* removed old artefacts [skip ci]

* works with compileTestJava

* restored metadata needed for codeQL and trusted-artifacts block for javadoc/sources



---------



[4844] Add encodingContext to TransactionEncoder and TransactionDecoder (#5820)

* Add decode type to TransactionDecoder

* Refactoring TransactionDecoder

* Invert methods order

* Use Transaction encoder instead of writeTo

* Move enter and leave list to inner method as pr suggestion

* Size calculation should use opaque bytes instead of rlp

---------






payload attributes: fix wrong warning and fail if beacon root is available before cancun (#5872)




Merge MutableAccount and EVMAccount (#5863)

Merge MutableAccount and EVMAccount functionalities by removing EVMAccount, all calls to getMutable, and the WrappedEVMAccount that was wrapping non-EVMAccounts in a mutable fashion.  Instead, use a MutableAccount in all cases an EVMAccount would have been used.  This also tends to reduce a level of layering in many places.



Add world context to transaction tracing API (#5836)

* Add world context to transaction tracing API



* Update changelog with PR ID



* Add the Transaction to traceEndTransaction



* Rebase on main



* Add receipt-linked information to the transaction tracer



* added test



---------






Bonsai based reference test worldstate (#5686)

* create a bonsai based reference test worldstate -> getOrCreate in BonsaiWorldStateUpdateAccumulator - do not throw if we discover an empty account in a non-null BonsaiValue<Account> -> add curentStateRoot to t8n -> storageEntriesFrom and streamAccounts implemented in BonsaiWorldStateKeyValueStorage -> add endKey version of streamFromKey
* bonsai fix for self-destruct and create2 at the same address and same block





Don't start BFT mining coordinators until initial sync has completed (#5861)

* Don't start BFT mining coordinators until initial sync has completed



* Fix unit tests



* Fix 'enable' logic



---------



display only peers ready for requets on ethstats (#5880)

* display only ready for requets peers in ethstats



* cast to int



---------






[MINOR] test RLP used for encode/decode blob tx should contain to field (#5883)

* validate to field on encode/decode for blob tx



* revert decode/encode checks - tis done later in tx validation



---------



Fix: correctly convert percentage options in TOML configuration file (#5886)



EIP7516 - Add BlobBaseFee opcode to Cancun EVM (#5884)



Fix snapsync heal (#5838)



Upgrade besu-native (#5893)

Upgrade besu-native to 0.8.2



Tune G1GC to reduce Besu memory footprint (#5879)



Add updated storage to evmtool json trace (#5892)

Add the EIP-3155 "storage" option to the standard tracer, with the caveat only updated storage is logged.



Update holesky with fixed extraData, genesis time, shanghaiTime (#5890)



[CHANGELOG] removed duplicated line (#5904)

* removed duplicated line [skip ci]



* fixed spelling on Holesky



---------

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
        Created At 2023-09-20 04:49:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5904" class=".btn">#5904</a>
            </td>
            <td>
                <b>
                    [CHANGELOG] removed duplicated line
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
        Created At 2023-09-20 02:49:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5903" class=".btn">#5903</a>
            </td>
            <td>
                <b>
                    update beacon root again
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Beacon root address has changed again - this PR is still draft so need to keep an eye on it leading up to devnet 9
https://github.com/ethereum/EIPs/pull/7672/files
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 23:46:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5901" class=".btn">#5901</a>
            </td>
            <td>
                <b>
                    Add FlatDbStrategy
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
This is a prerequisite PR for #5865 and #5887.  

It:
* expands the concept of FlatDbReaderStrategy to FlatDbStrategy, including write operations.
* adds getNearestTo implementation to SegmentedKeyValueStorage and its implementations
* adds getNearestTo test coverage and expands KeyValueStorage tests to SegmentedKeyValueStorage implementations

This PR will allow for parallel progress on SnapServer server and Bonsai Archive, and mitigate merge conflicts that would otherwise arise

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
related to #3165 and #5864
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 22:41:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5899" class=".btn">#5899</a>
            </td>
            <td>
                <b>
                    Update reference tests to 12.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description


Update reference tests to 12.4
* Some in-memory storage changed to ConcurrentMap
* exclude cancun from all EIP tests, EIP-4788 still in flux
* Add new fields to ReferenceTestEnv, and re-order the reflected constructor for clarity and ease of development.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
includes speculative changes for #5898 concurrency issue.  `services/kvstore/...` can be dropped out if there are other fixes, but transient failures result in blockchain and general state tests when removed
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 19:41:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5893" class=".btn">#5893</a>
            </td>
            <td>
                <b>
                    Upgrade besu-native to 0.8.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Upgrade besu-native to 0.8.2

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 15:03:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5892" class=".btn">#5892</a>
            </td>
            <td>
                <b>
                    Add updated storage to evmtool json trace
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

Add the EIP-3155 "storage" option to the standard tracer, with the caveat only updated storage is logged.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 03:27:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5891" class=".btn">#5891</a>
            </td>
            <td>
                <b>
                    add plugin API to enable plugins to validate transaction before they are added to the transaction pool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Adding a plugin API to enable plugins to validate of transactions entering the transaction pool
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 00:41:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5890" class=".btn">#5890</a>
            </td>
            <td>
                <b>
                    Update holesky with fixed extraData, genesis time, shanghaiTime
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Incorporates https://github.com/eth-clients/holesky/pull/73
and also @fab-10's changes from https://github.com/eth-clients/holesky/pull/72
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 21:44:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5889" class=".btn">#5889</a>
            </td>
            <td>
                <b>
                    Draft PR: Code storage by hash
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
Draft PR for storing code by hash instead of by address. This is needed snapsync as we need to be able to retrieve the code by hash.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixed #5388 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 07:02:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5887" class=".btn">#5887</a>
            </td>
            <td>
                <b>
                    SnapServer using FlatDB Strategy
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
Draft PR to implement SnapServer using FlatDB Strategy

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3165 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-16 12:49:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5886" class=".btn">#5886</a>
            </td>
            <td>
                <b>
                    Fix: correctly convert percentage options in TOML configuration file
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

Fix for a regression introduced by #5772 that causes the following exception when the option `tx-pool-limit-by-account-percentage` is defined as a number in the configuration file

```
TomlInvalidTypeException: Value of 'tx-pool-limit-by-account-percentage' is a float while processing argument at or before arg[0] '--config-file=./config.toml' in [--config-file=./config.toml]: org.apache.tuweni.toml.TomlInvalidTypeException: Value of 'tx-pool-limit-by-account-percentage' is a float
```

the fix is to simply convert percentage options to string when parsing the file
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 13:04:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5885" class=".btn">#5885</a>
            </td>
            <td>
                <b>
                    RPC - Implement Debug trace call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span><span class="chip">mainnet</span><span class="chip">RPC</span>
            </td>
            <td>
                ## PR description
Implement Debug trace call

## Fixed Issue(s)
fix #5747
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 09:05:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5884" class=".btn">#5884</a>
            </td>
            <td>
                <b>
                    EIP7516 - Add BlobBaseFee opcode to Cancun EVM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add BLOBBASEFEE to Cancun EVM

## Fixed Issue(s)
fixes #5869 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 05:59:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5883" class=".btn">#5883</a>
            </td>
            <td>
                <b>
                    [MINOR] test RLP used for encode/decode blob tx should contain to field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `to` field cannot be empty for blob tx so it doesn't make sense to check encoding / decoding without this

However that field being absent doesn't fail the tests because this is checked in the transaction validation -   https://github.com/hyperledger/besu/blob/4b2ef689c1f64e3fdb293dec826af1ad57e54fca/ethereum/core/src/main/java/org/hyperledger/besu/ethereum/mainnet/MainnetTransactionValidator.java#L299


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 02:49:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5882" class=".btn">#5882</a>
            </td>
            <td>
                <b>
                    [DO NOT MERGE] devnet8: correct address and modulus for beacon root
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Do not merge. This is a short time brach for devnet 8.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 23:28:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5880" class=".btn">#5880</a>
            </td>
            <td>
                <b>
                    display only peers ready for requets on ethstats
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Filter peer collection by those ready for connection. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 13:04:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5879" class=".btn">#5879</a>
            </td>
            <td>
                <b>
                    Tune G1GC to reduce Besu memory footprint
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

These flags have been suggested by @ahamlat , and we tested them for months now, they have the effect of reducing the off heap memory used by Besu, without affecting the overall performance.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 10:45:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5876" class=".btn">#5876</a>
            </td>
            <td>
                <b>
                    adds Matthew Whitehead as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I propose to add  @matthew1001 as a Besu project maintainer.

@matthew1001 contributed with many high quality commits:

- has implemented new JSON-RPC api endpoints, per execution api specs
- has improved error reporting in apis
- has improved configurability for non PoS networks

Here are [their past contributions on Besu project](https://github.com/hyperledger/besu/pulls?q=is:pr+author:matthew1001+is:closed).

Voting ends two weeks from today.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 17:20:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5875" class=".btn">#5875</a>
            </td>
            <td>
                <b>
                    init checkpoint state
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
        Created At 2023-09-13 17:06:32 +0000 UTC
    </div>
</div>

