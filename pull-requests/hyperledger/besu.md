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
                PR <a href="https://github.com/hyperledger/besu/pull/5686" class=".btn">#5686</a>
            </td>
            <td>
                <b>
                    Bonsai based reference test worldstate
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
@shemnon pointed out that the reference tests support in besu does not use bonsai worldstate, nor does evmtool.  This PR creates a bonsai-based worldstate and accumulator for ReferenceTestsWorldState.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 22:44:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5684" class=".btn">#5684</a>
            </td>
            <td>
                <b>
                    Update tuweni2.4.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Update Tuweni to 2.4.2.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 06:26:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5683" class=".btn">#5683</a>
            </td>
            <td>
                <b>
                    [4844] Add excessDataGas and dataGasUsed validation to EngineNewPayloadV3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add excessDataGas and dataGasUsed validation to EngineNewPayloadV3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 05:59:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5682" class=".btn">#5682</a>
            </td>
            <td>
                <b>
                    Introduce transaction validator interface (phase 2)
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

The focus of this PR is to complete the work started in #5673 and remove the odd `setPermissionTransactionFilter` from the interface.
The `setPermissionTransactionFilter` method is only relevant for private network when [permissioning](https://besu.hyperledger.org/stable/private-networks/concepts/permissioning) is enabled, so it make sense to have a dedicated validator for that, so `PermissionTransactionValidator` has been introduced to handle that use case, while it delegates all the other validations to `MainnetTransactionValidator`.
To obtain that, as common, another layer of indirection was required, since it is not possible to create the `PermissionTransactionValidator` when building the protocol schedule, due to a cyclic dependency, so the need for `TransactionValidatorFactory` that is available through the protocol schedule, and for efficiency create and memoize the actual transaction validator on first usage when all the required prerequisite, to build any kind of transaction validator, are satisfied.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 16:53:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5681" class=".btn">#5681</a>
            </td>
            <td>
                <b>
                    add global transaction to avoid worldstate inconsistencies 
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

This PR enables handling commits of the world state with a single transaction. This helps prevent inconsistencies between different columns in case of power failure or OOM, for example. With this PR, we will have a single global transaction for everything, and if anything goes wrong, all columns will be rollback.

Additionally, this PR removes the unused version 0 of the database, which adds unnecessary code.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 15:24:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5680" class=".btn">#5680</a>
            </td>
            <td>
                <b>
                    [4844] Fix Data Gas Price Calculation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This pull request addresses two issues: fixing the data gas price calculation and adjusting the genesis state methods to verify forks. The details of each issue are described below:

### Data Gas Price Calculation
The previous implementation of data gas price calculation had a flaw. It only considered the parent's excessDataGas to determine the dataPricePerGas, which overlooked the data gas used by the parent header itself. Consequently, when a large number of transactions were sent and the gas price increased, blocks were generated with transactions that should not have been included due to their price.

To rectify this, the calculation now incorporates both the parent's excessDataGas and the data gas used by the parent header. The code snippet from the specification is provided below:


```
def get_data_gasprice(header: Header) -> int:
    return fake_exponential(
        MIN_DATA_GASPRICE,
        header.excess_data_gas,
        DATA_GASPRICE_UPDATE_FRACTION
    )
```

This modification ensures that the assertion in block creation and transaction processing considers the correct data gas price, preventing inclusion of transactions with insufficient data gas price.

### Genesis State Verification for Cancun Fork
For the Cancun fork, there was an issue with the genesis state not including WithdrawsRoot in the genesis block. The problematic code snippet was as follows:

`return shanghaiTimestamp.getAsLong() == genesis.getTimestamp();`
To address this issue, the code has been updated as follows:

`return genesis.getTimestamp() >= shanghaiTimestamp.getAsLong();`

This change ensures that the genesis block's timestamp is greater than or equal to the shanghaiTimestamp, correctly reflecting the inclusion of WithdrawsRoot in the genesis state for the Cancun fork.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 13:07:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5679" class=".btn">#5679</a>
            </td>
            <td>
                <b>
                    Avoid doing two validations on transactionsRoot and ReceiptsRoot during sync
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

This PR enhances the Sync process by eliminating duplicate validations for transactions root and receipts root. We've noticed in CPU profiles during sync that receipts root and transactions root are calculated twice. The first time when data is retrieved from other peers, and the second time during block import when validating block body. This PR implements a mechanism to maintain a record of previously validated transactions and receipts roots, ensuring that redundant validations are avoided.

### **Sync time improvement (on a 4 vCPU/ 32 GiB RAM VM)**

<img width="1627" alt="image" src="https://github.com/hyperledger/besu/assets/5099602/8268a40d-627b-4a98-9eb8-e321a4010efc">

**Without this PR**
Checkpoint sync time : 19 hours 54 minutes

**With this PR**
 Checkpoint sync time : 16 hours 42 minutes

### **CPU profiling** 
We can notice in the profiling screenshots that Besu does the receipts root validation only once with this PR when getting the receipts from the peers.

**Before this PR**

<img width="1228" alt="image" src="https://github.com/hyperledger/besu/assets/5099602/63c05dc5-8ffe-48d5-b53b-20111f53094d">

**After this PR**

<img width="1367" alt="image" src="https://github.com/hyperledger/besu/assets/5099602/754c7b18-05f0-491f-ba4a-2ed1b25997a5">


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 12:56:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5678" class=".btn">#5678</a>
            </td>
            <td>
                <b>
                    Ethereum - migrated tests from Junit4 to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR removes junit4 dependency from ethereum modules
Converts junit4 tests to junit5 according to https://blogs.oracle.com/javamagazine/post/migrating-from-junit-4-to-junit-5-important-differences-and-benefits

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5564
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 07:06:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5677" class=".btn">#5677</a>
            </td>
            <td>
                <b>
                    [4844] [Hive] Fix for genesis mismatch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Fix from @spencer-tb 

https://github.com/hyperledger/besu/pull/5664#issuecomment-1620559037

> We recently added the hive pyspec simulator to https://hivecancun.ethdevops.io/, which runs the tests from https://github.com/ethereum/execution-spec-tests using the EngineAPI
> 
> In order to start running the tests the genesis state needs to include the `excessDataGas` and `dataGasUsed`, otherwise we get a genesis mismatch -> leading to a `SYNCING` status when adding the first block with `NewPayloadV3` via the EngineAPI, as opposed to a `VALID` or expected `INVALID` status.



> We recently added the hive pyspec simulator to https://hivecancun.ethdevops.io/, which runs the tests from https://github.com/ethereum/execution-spec-tests using the EngineAPI
> 
> In order to start running the tests the genesis state needs to include the `excessDataGas` and `dataGasUsed`, otherwise we get a genesis mismatch -> leading to a `SYNCING` status when adding the first block with `NewPayloadV3` via the EngineAPI, as opposed to a `VALID` or expected `INVALID` status.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 00:11:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5675" class=".btn">#5675</a>
            </td>
            <td>
                <b>
                    Upgrade BouncyCastle libraries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Upgrade bouncy castle to v1.75.  This involved a change in maven
coordinates for other modules.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 15:20:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5673" class=".btn">#5673</a>
            </td>
            <td>
                <b>
                    Introduce transaction validator interface (phase 1)
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

The main goal of this PR is the introduction of the `TransactionValidator` interface to pave the way for future simpler custom transaction validation necessary on private networks and/or specialized networks.
The work is not completed yet, and more PRs will be made, the next one will address the removal of the odd method `setPermissionTransactionFilter` from the interface

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 09:56:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5671" class=".btn">#5671</a>
            </td>
            <td>
                <b>
                    [4844] Add Engine Api  Cancun Acceptance Test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 22:28:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5670" class=".btn">#5670</a>
            </td>
            <td>
                <b>
                    Test updates for cancun execution-spec-tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Update t8n tool to support new fields (data gas related) for Cancun in the execution-spec-tests,
also, refactor so the t8n server benefits from the changes.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 14:11:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5669" class=".btn">#5669</a>
            </td>
            <td>
                <b>
                    Add genesis configuration isPoa() convenience function, and use it in validation of `--miner-enabled` option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR indirectly relates to issue https://github.com/hyperledger/besu/issues/5528.

The intention of the PR is to change the validation logic of the `--miner-enabled` option, particularly with regard to `--min-gas-price` option which is a common requirement for private POA chains.

Specifically, in the case where a POA consensus algorithm has been configured (`qbft`, `ibft2`, `ibft`, or `clique`) validation of options that would otherwise require `--miner-enabled` to be set, is skipped.

## Fixed Issue(s)
No specific issue is open for this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 13:14:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5668" class=".btn">#5668</a>
            </td>
            <td>
                <b>
                    [4844] Swap parameters order and remove unused method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

- Swap parameters order and 
- remove unused method
- move the method to a more relevant class
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 12:52:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5667" class=".btn">#5667</a>
            </td>
            <td>
                <b>
                    [4844] NewPayloadV3 - Add fork validation and fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

- This PR implements a fork validation for the newPayloadV3

Unrelated: 

-  Change the type of dataGasUsed to `Long` instead of `long`
- Add acceptance tests for Engine API  - Cancun
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 08:09:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5666" class=".btn">#5666</a>
            </td>
            <td>
                <b>
                    [POC] Comment out backwards sync for newPayload
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

Running a quick feasibility test based on https://github.com/hyperledger/besu/issues/5411#issuecomment-1600401704

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 01:57:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5665" class=".btn">#5665</a>
            </td>
            <td>
                <b>
                    Add Xlayered-tx-pool to the config log printout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Unrelated: clarify epoch length in javadoc

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
        Created At 2023-07-02 05:06:24 +0000 UTC
    </div>
</div>

