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
                    wip: add multi-platform support
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
                PR <a href="https://github.com/hyperledger/besu/pull/3478" class=".btn">#3478</a>
            </td>
            <td>
                <b>
                    Remove shutdown latch from BftProcessor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">consensus</span>
            </td>
            <td>
                We don't want BftMiningCoordinator.stop() to wait for BftProcessor to shutdown before calling shutdown on the BftExecutor.
This prevents BftMiningCoordinator from being able to be shutdown from the same thread.
We want to enable shutdown from the same thread to support migrating from one MiningCoordinator instance to another (IBFT -> QBFT).

This is the relevant discussion as to why the latch was originally added in: https://github.com/hyperledger/besu/pull/104#discussion_r334705699

I believe the latch is unnecessary because BftExecutors.stop() (which calls bftProcessExecutor.shutdownNow) should be sufficient to safely prevent any further tasks from being accepted, whilst BftExecutors.awaitStop() (calling bftProcessExecutor.awaitTermination()) gives the current task(s) a chance to finish.

This PR is most if not all of the solution to https://github.com/hyperledger/besu/issues/3003
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 04:39:13 +0000 UTC
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
                    Initial commit for trace_get implementation. No tests.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mark Terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Implementation for trace_get.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3464" class=".btn">#3464</a>
            </td>
            <td>
                <b>
                    Change chat pointers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hyperledger has moved to Discord.

Signed-off-by: Ry Jones <ry@linux.com>

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-20 17:16:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3462" class=".btn">#3462</a>
            </td>
            <td>
                <b>
                    Add components to handle the transition from PoW to PoS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Code originally written by garyschulte on the merge branch.

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

This PR is built on top of #3461 that should be reviewed first

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-18 16:09:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3461" class=".btn">#3461</a>
            </td>
            <td>
                <b>
                    Add The Merge core components
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                List of components: controller builder, protocol schedule,
coordinator, block creator and processor.

Code originally written by garyschulte on the merge branch.
Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

This PR is built on top of #3454 that should be reviewed first

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
        Created At 2022-02-18 14:18:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3459" class=".btn">#3459</a>
            </td>
            <td>
                <b>
                    trace_rawTransaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Json RPC endpoint and test files for trace_rawTransaction

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-18 05:08:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3458" class=".btn">#3458</a>
            </td>
            <td>
                <b>
                    Update discovery to 22.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Update to the latest version of discovery (22.2.0). Main change is to switch RLP parsing to use tuweni-rlp instead of web3j which avoids needing to create intermediate objects during the parsing process.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-18 01:31:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3457" class=".btn">#3457</a>
            </td>
            <td>
                <b>
                    one more discord link and a typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed a typo
And a discord link

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-18 01:02:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3455" class=".btn">#3455</a>
            </td>
            <td>
                <b>
                    update version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

update version 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 15:05:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3454" class=".btn">#3454</a>
            </td>
            <td>
                <b>
                    Add header validation rules needed to validate The Merge blocks
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

This is built on top of another PR that should be merged first https://github.com/hyperledger/besu/pull/3453

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 14:38:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3453" class=".btn">#3453</a>
            </td>
            <td>
                <b>
                    Add PostMergeContext that will stop syncing after the swith to PoS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Code originally written by garyschulte and gezero on the merge branch.
Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

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
        Created At 2022-02-17 14:26:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3451" class=".btn">#3451</a>
            </td>
            <td>
                <b>
                    Rename MergeOptions to MergeConfigOptions to follow the standard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

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
        Created At 2022-02-17 11:02:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3448" class=".btn">#3448</a>
            </td>
            <td>
                <b>
                    update version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

change gradle.properties to snapshot version

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 01:17:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3447" class=".btn">#3447</a>
            </td>
            <td>
                <b>
                    merge of forkchoice and kiln changes back to main
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
* merge forkchoiceUpdated method and test coverage to main
* merge kiln spec changes to main for previously merged json-rpc methods


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
addresses all but newPayload for #2965 


## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 00:29:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3446" class=".btn">#3446</a>
            </td>
            <td>
                <b>
                    Fix typo in method name
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
        Created At 2022-02-16 22:06:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3445" class=".btn">#3445</a>
            </td>
            <td>
                <b>
                    Update Changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Update changelog for 22.1.0. This includes consolidating all RC changes
into the main release.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 18:17:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3444" class=".btn">#3444</a>
            </td>
            <td>
                <b>
                    New MutableBlockchain method rewindToBlock by hash prerequisite for T…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …he Merge

Code originally written by garyschulte on the merge branch
Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 14:35:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3442" class=".btn">#3442</a>
            </td>
            <td>
                <b>
                    New release 22.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry picked commits: 
- 1f234f23f
- 117b1b133
- 68f6fcd10
- 21f7fba7e
- 89768844f
- 0f798dd44
- 764d80abc
- e32f284cf
- da6adecb5
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 03:51:47 +0000 UTC
    </div>
</div>

