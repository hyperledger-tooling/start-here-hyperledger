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
                PR <a href="https://github.com/hyperledger/besu/pull/5931" class=".btn">#5931</a>
            </td>
            <td>
                <b>
                    BlockTransactionSelector refactoring
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
`BlockTransactionSelector` refactoring:

- Extract `TransactionSelectionResults` to its own class.
- Extract Transaction Selection Criteria and selection logic out of the `BlockTransactionSelector` to their own classes
- `BlockTransactionSelector` will use a list of selectors to evaluate the transaction
- Similar to selectors that will evaluate a transaction

Next steps:

- Expose `TransactionProcessingResult` (or at least a part of it the to Plugin interface)
- Abstract the transaction selectors and external transaction selectors so they share the same logic
- Add a way to get the `OperationTracer` from the TPR and pass it to the plugin 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-25 03:22:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5930" class=".btn">#5930</a>
            </td>
            <td>
                <b>
                    Add parameters to EVM library fluent API
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

Add the ability to configure more parameters in the fluent API. Specifically contract address, coinbase, difficulty, mixHash/prevRandao, baseFee, block number, timestamp, gas limit, previous block hashes, and versioned hashes.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-22 15:28:35 +0000 UTC
    </div>
</div>

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
                    Always enforce promotion filter for transactions in the prioritized layer
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

This PR is built on top of #5920, so please check it first ([relative changes](https://github.com/fab-10/besu/compare/fab-10:besu:txpool-promotion-performance...prioritized-promotion-filter2))

This PR is preparatory for more work on prioritizing local txs, that consist in more small PRs that have been split to make it easier to review.
Before the PR, the prioritized layer also kept txs that could not be selected to be included in the next block, because as far as there was still space txs were added and kept there, regardless they were or not satisfying the promotion filter anymore.
This PR improves the content of the prioritized layer, keeping there only txs that always satisfy the promotion filter, and thus are candidate for inclusion in the next block, this avoid to waste some work during txs selection, and pave the way for an easier prioritization of local txs.
Currently the promotion filter says that a tx is willing to pay at list the base fee, on base fee market network, otherwise is always true.

Simulation of block production shows no regression, actually metrics about number of txs in the block, block value and gas used are, on average, better with this PR vs 23,7,2 version:
![image](https://github.com/hyperledger/besu/assets/91944855/309a58ac-838e-4da6-b3e7-703b9ce5644b)

![image](https://github.com/hyperledger/besu/assets/91944855/3a019711-770c-4d26-b1b7-7555d8ba2b71)

![image](https://github.com/hyperledger/besu/assets/91944855/ddad0bc1-9ece-4507-99f8-efa38a46db6a)



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

During the implementation of #5921, a performance issue surfaced in the way the promotion of transactions, from lower layers, was implemented.
The issue was that, to keep the code simple, the promotion was done for one tx at once, but with the improvement on the prioritized layer done #5921, this approach is no more practical since result in a quadratic complexity (number of confirmed txs per number of senders in the ready layer), so the solution is to do the promotion only once after all the confirmed txs have been processed, so the time is linear.

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
PR that adds getproof for Bonsai. With this implementation, we can serve the getproof for historical states and not just the head.
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

