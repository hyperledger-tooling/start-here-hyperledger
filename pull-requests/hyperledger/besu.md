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
Ensure besu correctly checks for latest ancestor before checking before checking if a block descends from terminal.  

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

