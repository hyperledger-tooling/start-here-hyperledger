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
                PR <a href="https://github.com/hyperledger/besu/pull/5674" class=".btn">#5674</a>
            </td>
            <td>
                <b>
                    Txvalidator builder
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
        Created At 2023-07-05 14:56:59 +0000 UTC
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
                    Comment out backwards sync for newPayload
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

