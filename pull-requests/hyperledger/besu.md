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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5664" class=".btn">#5664</a>
            </td>
            <td>
                <b>
                    [4844] Read ExcessDataGas and ExcessDataGas from genesis if Cancun is present
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix for genesis mismatch

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-02 04:49:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5663" class=".btn">#5663</a>
            </td>
            <td>
                <b>
                    [4844] Check params earlier and move blob validation to a new method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Check the params earlier and move blob validation to a new method

In case CL sends a payload with invalid blob params for a known header, we should return invalid.

Expected Behaviour: return invalid

Actual Behaviour: Returns are valid because we have already seen that payload.

This PR moves the validation earlier in the flow and encapsulates the validation login into a method for readability.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-30 07:11:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5662" class=".btn">#5662</a>
            </td>
            <td>
                <b>
                    Extend OperationTracer with new methods
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

This PR extends the `OperationTracer` with 2 new methods:

* traceStartTransaction, which complements the existing traceEndTransaction
* isExtendedTracing, which returns `false` by default, but can be overrriden by other tracer implementations

Extended tracing is needed in cases where the current tracing implementations does not provide sufficient insight into a transaction. This is for example required for zkEVM implementations as those often require a more detailed insight into a transaction for the proof generation. This PR introduces extended tracing in case of a successful contract creation. More extending tracing will be added in future PRs.

Further the plugin API for tracing is extended as well. It adds 2 new methods:

* traceStartBlock
* traceEndBlock

Both take a block header and a block body as a parameter. It was required to use those 2 instead of a `Block` object, because the latter is causing circular dependency issues that would require a very big refactoring to resolve them.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-30 05:49:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5661" class=".btn">#5661</a>
            </td>
            <td>
                <b>
                    Add --amend to docker manifest create to fix docker latest tag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We need to replace previous release's latest tag. Might be broken due to a recent change in the docker command implementation

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-30 03:58:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5660" class=".btn">#5660</a>
            </td>
            <td>
                <b>
                    Put download links into CHANGELOG and do some clean up
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
        Created At 2023-06-30 03:30:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5659" class=".btn">#5659</a>
            </td>
            <td>
                <b>
                    Only update peer with the first and last block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
We only need to update the peers chain state with the highest block header, which is the first or the last block in the list. Currently we are trying to update with every block header, which can be 200 or so.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-30 00:06:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5657" class=".btn">#5657</a>
            </td>
            <td>
                <b>
                    [4844] Acceptance Test - Update block hash with correct value 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">4844</span>
            </td>
            <td>
                ## PR description
Update the acceptance test with the right hash value since the header now also has dataGasUsed
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-29 08:47:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5656" class=".btn">#5656</a>
            </td>
            <td>
                <b>
                    Add hooks to AbstractCreateOperation for library users
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

Add hooks for a successful contract create, a failed contract create, and an invalid contact create. Users of the library will be able to customize create responses without having to replace core logic.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 22:41:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5654" class=".btn">#5654</a>
            </td>
            <td>
                <b>
                    DataGas all the longs!!!!
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use the DataGas type instead of longs everywhere possible.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 15:41:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5653" class=".btn">#5653</a>
            </td>
            <td>
                <b>
                    [WIP] Store RLP encoding to avoid encoding operations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">performance</span><span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
The goal of this PR is to store RLP encoding bytes insides different objects  (transaction, transactionReceipt, BlockBody and BlockHeader) to avoid encoding operations when we need the get the RLP encoding.

This PR has also an improvement on Sync process to avoid transaction root validation and receipt root validation twice.

Before this PR
![image](https://github.com/hyperledger/besu/assets/5099602/e4521b7e-cbf4-4db6-99e9-bed70453b120)

After this PR (We can notice that receipts root validation appears only once)
![image](https://github.com/hyperledger/besu/assets/5099602/67df51a6-38d6-4290-ad52-aa9edb395c81)


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 13:07:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5652" class=".btn">#5652</a>
            </td>
            <td>
                <b>
                    Prepare for version 23.4.5-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
prepare for version 23.4.5-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 07:39:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5651" class=".btn">#5651</a>
            </td>
            <td>
                <b>
                    Release 23.4.4
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

Force pushed 23.4.3 changes (and the extra 23.4.4-SNAPSHOT commit) onto release-23.4.x before making this PR.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 06:03:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5650" class=".btn">#5650</a>
            </td>
            <td>
                <b>
                    [4844] Add Data Gas Excess Validation to the Header Validations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Add dataGasExcess header validation according to https://eips.ethereum.org/EIPS/eip-4844

>     # check that the excess data gas was updated correctly
>     assert block.header.excess_data_gas == calc_excess_data_gas(block.parent.header)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 06:02:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5648" class=".btn">#5648</a>
            </td>
            <td>
                <b>
                    Release 23.4.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.4.4
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 01:21:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5647" class=".btn">#5647</a>
            </td>
            <td>
                <b>
                    Fix getAccountProof for Bonsai
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR fix the eth_getProof RPC method when using Bonsai by adding the worldStateProof to BonsaiWorldStateProvider.
By passing a snapshot of the ws that we want the proof for the BonsaiWorldStateProvider should be able to make normal usage of the worldStateProof to generate the proofs.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Part of #5377 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 00:53:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5644" class=".btn">#5644</a>
            </td>
            <td>
                <b>
                    init snap opti
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
        Created At 2023-06-27 08:25:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5643" class=".btn">#5643</a>
            </td>
            <td>
                <b>
                    [4844] CancunGasCalculator ->  Fix Excess Data Gas Calculation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fixing the formula according to `calc_excess_data_gas` in https://eips.ethereum.org/EIPS/eip-4844
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 06:38:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5642" class=".btn">#5642</a>
            </td>
            <td>
                <b>
                    [4844] Set CancunGasCalculator maxPrecompile to KZG_POINT_EVAL
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Cancun implements a new precompile and the gas calculator needs to consider its new address.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 04:13:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5641" class=".btn">#5641</a>
            </td>
            <td>
                <b>
                    Remove BLS12 from cancun
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

BLS12 signatures were speculatively added in cancun in late 2022.  This is no longer accurate.  Move the implementation to the "Future_EIPs" fork so that it will remain testable and not accidentally get included accidentally.  Also add missing fluent APIs.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 00:18:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5640" class=".btn">#5640</a>
            </td>
            <td>
                <b>
                    Eth/68: treat transaction size as scalar unsigned int
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamChupa</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Align Besu to what other clients are doing, treating the sizes as an array of scalar ints and not 4 bytes, this also prevent being disconnected from Geth due to `invalid-message` error:

```
DEBUG[06-19|15:15:40.347] Ethereum peer connected                  id=a1697db12e1f2986 conn=inbound name=besu/v23.4.0/linux-x...
DEBUG[06-19|15:15:40.360] Message handling failed in `eth`         id=a1697db12e1f2986 conn=inbound err="invalid message: message msg #8 (157028 bytes): invalid message: (code 8) (size 157028) rlp: non-canonical integer (leading zero bytes) for uint32, decoding into (eth.NewPooledTransactionHashesPacket68).Sizes[0]"
DEBUG[06-19|15:15:40.360] Removing p2p peer                        peercount=10 id=a1697db12e1f2986 duration=12.956ms     req=false err="invalid message: message msg #8 (157028 bytes): invalid message: (code 8) (size 157028) rlp: non-canonical integer (leading zero bytes) for uint32, decoding into (eth.NewPooledTransactionHashesPacket68).Sizes[0]"
```

Contacting the author of the EIP for making it clearer in which data type is used for this message, see https://github.com/ethereum/EIPs/pull/7233

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 14:21:49 +0000 UTC
    </div>
</div>

