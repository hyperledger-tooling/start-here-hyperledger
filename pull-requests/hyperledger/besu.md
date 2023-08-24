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
                PR <a href="https://github.com/hyperledger/besu/pull/5794" class=".btn">#5794</a>
            </td>
            <td>
                <b>
                    Make checkSpdxHeader task cross platform
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

Another small PR to allow running checkSpdxHeader task on Windows

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 08:55:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5793" class=".btn">#5793</a>
            </td>
            <td>
                <b>
                    Remove versionedHashes from EngineNewPayload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove versionedHashes from EngineNewPayload. 

It does not belong to the payload parameter:
https://github.com/ethereum/execution-apis/blob/main/src/engine/cancun.md#executionpayloadv3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 05:41:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5792" class=".btn">#5792</a>
            </td>
            <td>
                <b>
                    EngineNewPayload - Validate parameters before fork validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Parameters validation should occur before fork validation

> Specification
> This method follows the same specification as [engine_newPayloadV2](https://github.com/ethereum/execution-apis/blob/main/src/engine/shanghai.md#engine_newpayloadv2) with the addition of the following:
> 
> 1. Client software MUST check that provided set of parameters and their fields strictly matches the expected one and return -32602: Invalid params error if this check fails. Any field having null value MUST be considered as not provided.
> 
> 2. Client software MUST return -38005: Unsupported fork error if the timestamp of the payload does not fall within the time frame of the Cancun fork.
> ...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 05:38:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5790" class=".btn">#5790</a>
            </td>
            <td>
                <b>
                    Example
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
        Created At 2023-08-23 14:44:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5789" class=".btn">#5789</a>
            </td>
            <td>
                <b>
                    Make referencetests build script Windows friendly
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

#5774 broken builds on Windows due to the different separation char, this PR just replace the '/' with the system separator char as provided by the jvm

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 10:05:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5787" class=".btn">#5787</a>
            </td>
            <td>
                <b>
                    fix #5744: Incorrect ForkId when first fork timestamp matches genesis timestamp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
If the genesis timestamp equaled the first timestamp fork an additional ForkId was added, which was incorrect.

## Fixed Issue(s)
fixes #5744
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 06:43:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5786" class=".btn">#5786</a>
            </td>
            <td>
                <b>
                    fix excess blob gas calculation when creating blobs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This fixes an issue where we were calculating the excess blob gas in a wrong way when generating a block proposal.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 01:32:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5783" class=".btn">#5783</a>
            </td>
            <td>
                <b>
                    adds manifestDocker task to release workflows, renames some vars in b…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …uild.gradle for clarity

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
        Created At 2023-08-22 17:11:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5780" class=".btn">#5780</a>
            </td>
            <td>
                <b>
                    fix: added shouldOverrideBuilder field to engine_getPayloadV3 response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                simply default to false for now. 

This should fix some failing hive tests.

fixes #5739 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-21 23:59:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5779" class=".btn">#5779</a>
            </td>
            <td>
                <b>
                    update changelog and version for 23.7.2-SNAPSHOT
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
title says it all, update version for 23.7.2-SNAPSHOT

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-21 17:40:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5778" class=".btn">#5778</a>
            </td>
            <td>
                <b>
                    Release 23.7.1
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
bump version after 23.7.1-RC2 burn-in

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-21 16:20:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5776" class=".btn">#5776</a>
            </td>
            <td>
                <b>
                    fix snapsync issue with forest
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

Fixing an issue during snapsync with forest related to the heal step

the step checking whether the node existed or not during the healing process could lead to a null pointer exception due to the null nodeHash, which was only utilized within the context of forest.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-21 08:27:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5774" class=".btn">#5774</a>
            </td>
            <td>
                <b>
                    Add EIPTests to ReferenceTests
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

Add the EIPTests directory to the set of reference tests.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 22:03:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5772" class=".btn">#5772</a>
            </td>
            <td>
                <b>
                    Layered txpool by default and txpool options hoverhaul
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

This PR started with the goal to switch to the new layered by default, adding the possibility to select the old implementation if needed, introducing a new option `--tx-pool` that can take the values `layered` (default) and `legacy`, all the previously unstable options for the layered pool `--tx-pool-layer-max-capacity`, `--tx-pool-max-prioritized`, `--tx-pool-max-future-by-sender` are not stable.
Options specific to each implementation have been grouped, also in the help section, and validation has been added to fail in case options for a specific implementation are misused with the other implementation.

While implementing this, I found that the txpool options were a bit messy, stable and unstable options mixed, many options cluttering `BesuCommand` and the presence of boilerplate (and error prone) code, so I decided to use this PR to also review, clean and improve the code:
- to move all the txpool options away from `BesuCommand` and split them correctly between stable and unstable, 
- made `getCLIOptions` to dynamically generate its output, via reflection, avoiding to manually add, and then maintain, any option, that is error prone. Most of the changes are related to this feature, that inspect by reflection the options in the class. Since these classes are only used at startup or during unit tests the performance of the reflection should not be an issue
- made the custom converters to return directly the high level type instead of the raw type, that seems the right way to use them.
- fixed some issues that happens when using the layered txpool by default in tests.

If the work done for txpool options, is found to be effective, then I can apply the same to other groups of options to clean and uniform them.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 14:32:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5771" class=".btn">#5771</a>
            </td>
            <td>
                <b>
                    Add eth_getBlockReceipts() JSON/RPC method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
Adds `eth_getBlockReceipts` JSON/RPC method as described by Ethereum API specification https://github.com/ethereum/execution-apis/pull/438

**Notes for PR reviewer & docs**:

- The specification says that the correct response for a block that cannot be found is an empty array, e.g. https://github.com/ethereum/execution-apis/blob/main/tests/eth_getBlockReceipts/get-block-receipts-future.io Besu  appears to have a convention of returning a `-32000` error code with message `Block not found` for such cases. I have done the same with this new JSON/RPC method but welcome any thoughts on this from the PR reviewer.
- I don't think this query requires any changes/additions to graphql. The current schema covers the basic EVM objects (block, transaction, log etc) and is already designed to provide an alternative way of doing what this new JSON/RPC method adds (getting all receipts for a block in a single call) so I haven't made any graphql changes.

## Fixed Issue(s)
Closes https://github.com/hyperledger/besu/issues/5751
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 12:22:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5768" class=".btn">#5768</a>
            </td>
            <td>
                <b>
                    Forkchoice v3
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
fixes #5735 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 14:16:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5766" class=".btn">#5766</a>
            </td>
            <td>
                <b>
                    Issue 5719 - remove Pretty JSON and make it user configurable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span><span class="chip">mainnet</span><span class="chip">RPC</span><span class="chip">ux</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Added --pretty-json-enabled as CLI option as it was asked in the issue mentioned bellow.

Here I attached an example with the output of a RPC request when Besu was ran with --pretty-json-enabled (first case) and without the argument in second case:
<img width="1255" alt="Screenshot 2023-08-17 at 16 44 00" src="https://github.com/hyperledger/besu/assets/99179176/e8e57de7-6afe-460c-a295-ad97f37dea42">


## Fixed Issue(s)
Fixes #5712 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 13:55:11 +0000 UTC
    </div>
</div>

