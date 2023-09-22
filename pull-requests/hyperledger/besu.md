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
                PR <a href="https://github.com/hyperledger/besu/pull/5929" class=".btn">#5929</a>
            </td>
            <td>
                <b>
                    [4844] Fix some Devnet9 Hive tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix null latest valid hash when validation blobs/expected hashes
Fix HISTORICAL_ROOTS_MODULUS used by hive/devnet 9
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-22 07:45:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5923" class=".btn">#5923</a>
            </td>
            <td>
                <b>
                    Add Cancun GraphQL fields
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

Add the fields for Blobs into the GraphQL service.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 17:31:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5921" class=".btn">#5921</a>
            </td>
            <td>
                <b>
                    Prioritized promotion filter2
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
        Created At 2023-09-21 16:35:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5920" class=".btn">#5920</a>
            </td>
            <td>
                <b>
                    Improve performance when promoting transaction from next layers
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
        Created At 2023-09-21 16:33:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5919" class=".btn">#5919</a>
            </td>
            <td>
                <b>
                    add get proof for bonsai
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
PR that adds the getproof for Bonsai. With this implementation, we can serve the getproof for historical states and not just the head.
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5874
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 07:34:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5918" class=".btn">#5918</a>
            </td>
            <td>
                <b>
                    [MINOR] Block number param additional test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Just an additional test to prove that hex and binary are both supported at this level
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 06:34:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5917" class=".btn">#5917</a>
            </td>
            <td>
                <b>
                    fix geth rlpx ping command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
The geth cmd 
./build/bin/devp2p rlpx ping enodeAddress
expects the client with address enodeAddress to respond with a HelloMessage right after successfully receiving the handshake message from the initiator.
Existing behaviour in Besu is to wait for the HelloMessage from the initiator before sending the HelloMessage back.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 05:45:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5916" class=".btn">#5916</a>
            </td>
            <td>
                <b>
                    renamed PayloadTuple and made a separate class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                adds flexibility for adding more info to the Payload object eg OperationTracer to be used by plugins
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 02:42:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5913" class=".btn">#5913</a>
            </td>
            <td>
                <b>
                    Bump version to 23.7.4-SNAPSHOT
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
        Created At 2023-09-20 20:04:50 +0000 UTC
    </div>
</div>

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
                    [4788] update beacon root address to latest - post audit tweaks
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

