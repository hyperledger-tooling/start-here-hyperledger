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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3494" class=".btn">#3494</a>
            </td>
            <td>
                <b>
                    [MINOR] remove orion refs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Removed some orion references

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 02:44:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3493" class=".btn">#3493</a>
            </td>
            <td>
                <b>
                    3378 ws engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

## PR description
Implements the engine API via websockets.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #3378 

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 01:32:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3492" class=".btn">#3492</a>
            </td>
            <td>
                <b>
                    Renamed OP code RANDOM to PREVRANDAO
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## Fixed Issue(s)
fixes #3489 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 15:19:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3486" class=".btn">#3486</a>
            </td>
            <td>
                <b>
                    Handle TTD and mining pre and post merge 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Correctly and consistently handle mining pre/post merge for PoW and Clique networks.  The majority of this PR is code from the merge branch which needed some 'treatment' in order to not cause regressions in behavior on main.

* for clarity, rename isStoppedAtTerminalDifficulty to hasReachedTerminalDifficulty 
* use AtomicReference for PostMergeContext rather than synchronized
* add mining parameter override for consensus mechanisms that mine regardless of miningParameters
* merge parameter validation from `merge` branch which allows mining parameters without PoW mining (if merge is enabled)
* merge fix for optional in TxPoolEvictionService
* fix for ancestorIsValidTerminalProofOfWork in MergeCoordinator when close to TTD
* address Rayonism tech-debt, use setBlockChoiceRule at TTD rather than disabling reorg behavior entirely pre-merge


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2898 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 03:11:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3485" class=".btn">#3485</a>
            </td>
            <td>
                <b>
                    Remove deprecated open telemetry proto dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Needed to add jaeger-proto dependency as per breaking changes info here https://github.com/open-telemetry/opentelemetry-java/releases/tag/v1.7.0

Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

See #3406 
Also updated grpc 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 00:56:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3483" class=".btn">#3483</a>
            </td>
            <td>
                <b>
                    Upgrade EnodeURL builder strategy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prioritize EnodeDNS in Enode builder to solve #3482 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 15:50:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3481" class=".btn">#3481</a>
            </td>
            <td>
                <b>
                    Feat: add multi-platform support
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
use buildx on linux AMD64 host to build docker image for platform amd64 & arm64
  - base image `ubuntu` support `amd64` `arm64` `riscv64` & `riscv64`
  - base image `ghcr.io/graalvm/graalvm-ce:ol7-java11` only support  `amd64` & `arm64`
  - Gitlab docker registry is used in testing

## To Do (s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
 -  integrate with CICD pipeline, e.g. `.CircleCI` & `Github Actions`

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 10:51:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3479" class=".btn">#3479</a>
            </td>
            <td>
                <b>
                    Additional trace_transaction tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added some more trace_transaction tests generated from 
https://github.com/ConsenSys/json-rpc-conformance-test-utils/pull/18

Note: some of these tests fail. I think it's just besu puts in an extra field for contract creation which OE does not
"[creationMethod" : "create",

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 06:21:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3477" class=".btn">#3477</a>
            </td>
            <td>
                <b>
                    trace_get 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mark Terry <mark.terry@consensys.net>

## PR description
Implementation for trace_get API.
* exclude revertReason from result (matches Besu trace_call and openethereum)

Note this implementation matches openethereum behaviour except for:
* we manually added `creationMethod` to test files even though openethereum 3.2.5 does not include this field (this matches Besu trace_transaction implementation which also includes the `creationMethod` field)

See #2889 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 04:30:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3476" class=".btn">#3476</a>
            </td>
            <td>
                <b>
                    Add some thread names for debugging clarity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BFT executor threads include IBFT or QBFT to help with the IBFT -> QBFT migration.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 04:14:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3475" class=".btn">#3475</a>
            </td>
            <td>
                <b>
                    QBFT out of early access
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This is the changlelog update that publicises that QBFT consensus algorithm is now production ready.

Also fixing some typos (fixes #3452)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 00:56:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3474" class=".btn">#3474</a>
            </td>
            <td>
                <b>
                    use med executor for quorum ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

The nightly CI failed overnight https://app.circleci.com/pipelines/github/hyperledger/besu/13408/workflows/e13faa55-846d-40cb-a18a-cb96eeff6d2f/jobs/74709
So this PR is 
* changing the executor back to the machine executor that it was using before
* changing from XL to MED
* removing extra gradle workers config

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 23:01:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3473" class=".btn">#3473</a>
            </td>
            <td>
                <b>
                    MERGE: engine_exchangeTransitionConfigurationV1 API
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

Implements the `engine_exchangeTransitionConfigurationV1` API endpoint according to [specification](https://github.com/ethereum/execution-apis/blob/main/src/engine/specification.md#engine_exchangetransitionconfigurationv1). It is part of the Kiln v2 spec.

## Fixed Issue(s)
fixes #3471 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 20:11:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3472" class=".btn">#3472</a>
            </td>
            <td>
                <b>
                    Migrate JumpDestCache to CodeCache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Migrate the jump dest analysis cache into a more generic code cache that
lives inside the EVM.

This is in preparation for Ethereum Object Formats where a string of
code may be treated differently depending on what EVM version is
executing the code. Newer versions will also have difference analyses to
run that will need different backing data structures.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 15:42:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3470" class=".btn">#3470</a>
            </td>
            <td>
                <b>
                    Execution specific RPC endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Code originally written by jflo on the merge branch.

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 10:44:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3468" class=".btn">#3468</a>
            </td>
            <td>
                <b>
                    WIP | Feature/trace callmany
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WIP
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 04:51:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3467" class=".btn">#3467</a>
            </td>
            <td>
                <b>
                    Quorum mode ATs - don't run in parallel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span>
            </td>
            <td>
                Quorum ATs do not run well in parallel. This PR removes the parallel gradle flag. Aiming to reduce flakiness of these tests.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-20 23:31:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3466" class=".btn">#3466</a>
            </td>
            <td>
                <b>
                    Separate CI steps for DCO and spotless checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will make it easier for PR authors (especially community members) to see what's failed.
See #3456 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-20 22:38:03 +0000 UTC
    </div>
</div>

