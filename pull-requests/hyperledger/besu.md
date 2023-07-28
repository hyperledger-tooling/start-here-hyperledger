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
                PR <a href="https://github.com/hyperledger/besu/pull/5727" class=".btn">#5727</a>
            </td>
            <td>
                <b>
                    Make smart contract permissioning features work with london fork
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Override the transactionSimulator's default TransactionValidationParams with one that allows for exceeding the account balance (which effectively zeros the baseFee). This mimics the way that eth_estimateGas and eth_call are implemented. Similar change to #5277

Update ATs to use londonBlock (existing genesis allocs necessitate zeroBaseFee as well)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-28 08:26:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5726" class=".btn">#5726</a>
            </td>
            <td>
                <b>
                    Correctly cache the TransactionValidator instance on creation
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

in #5682 `Suppliers.memoize` was misused and so a new instance was created at every `get` invocation, instead of correctly return the cached instance created at creation time

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 18:04:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5724" class=".btn">#5724</a>
            </td>
            <td>
                <b>
                    Consolidated EIP-4844
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
- refactors Engine API tests to reuse OR override prior versions
- new DataGas type for tracking block cost for 4844 data
- new VersionedHash type to reflect that a versioned hash is not quite a pure sha256
- incorporates wrapped jc-kzg library for KZG point evaluations
- New transaction type, and domain objects for constituent parts to represent the Blobs, KZGCommitments, and Proofs used for 4844
- RLP encoders and decoders to support new transaction type
- gas pricing calculators for the new type of gas
- plugin-api version was changed
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 15:53:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5723" class=".btn">#5723</a>
            </td>
            <td>
                <b>
                    Prepare for version 23.7.1-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 23.7.1-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 00:13:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5722" class=".btn">#5722</a>
            </td>
            <td>
                <b>
                    Release 23.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.7.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 23:05:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5720" class=".btn">#5720</a>
            </td>
            <td>
                <b>
                    ethereum/part8 - migrated tests from Junit4 to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR removes junit4 dependency from ethereum/retesteth, ethereum/rlp, ethreum/trie, ethereum/verkletrie files

Split part 8 PR from https://github.com/hyperledger/besu/pull/5678

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5564
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 21:07:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5719" class=".btn">#5719</a>
            </td>
            <td>
                <b>
                    ethereum/permissioning - migrated tests from Junit4 to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR removes junit4 dependency from ethereum/permissioning files

Split part 7 PR from https://github.com/hyperledger/besu/pull/5678

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5564
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 21:01:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5718" class=".btn">#5718</a>
            </td>
            <td>
                <b>
                    ethereum/p2p - migrated tests from Junit4 to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR removes junit4 dependency from ethereum/p2p files

Split part 6 PR from https://github.com/hyperledger/besu/pull/5678

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5564
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 20:56:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5717" class=".btn">#5717</a>
            </td>
            <td>
                <b>
                    ethereum/part5 - migrated tests from Junit4 to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR removes junit4 dependency from ethereum/ethstats, ethereum/evmtool, ethereum/mock-p2p files

Split part 5 PR from https://github.com/hyperledger/besu/pull/5678 

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5564
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 20:52:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5716" class=".btn">#5716</a>
            </td>
            <td>
                <b>
                    ethereum/eth - migrated tests from Junit4 to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR removes junit4 dependency from ethereum/eth files

Split part 4 PR from https://github.com/hyperledger/besu/pull/5678

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5564
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 20:36:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5715" class=".btn">#5715</a>
            </td>
            <td>
                <b>
                    ethereum/core - migrated tests from Junit4 to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR removes junit4 dependency from ethereum/core files

Split part 3 PR from https://github.com/hyperledger/besu/pull/5678

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5564
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 20:32:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5714" class=".btn">#5714</a>
            </td>
            <td>
                <b>
                    ethereum/blockcreation - migrated tests from Junit4 to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR removes junit4 dependency from ethereum/blockcreation files

Split part 2 PR from https://github.com/hyperledger/besu/pull/5678

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5564
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 20:25:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5713" class=".btn">#5713</a>
            </td>
            <td>
                <b>
                    ethereum/api - migrated tests from Junit4 to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR removes junit4 dependency from ethereum/api files
Converts junit4 tests to junit5 according to https://blogs.oracle.com/javamagazine/post/migrating-from-junit-4-to-junit-5-important-differences-and-benefits

Split part 1 PR from https://github.com/hyperledger/besu/pull/5678

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5564
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 20:18:47 +0000 UTC
    </div>
</div>

