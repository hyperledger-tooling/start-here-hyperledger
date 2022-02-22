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
                WIP code and test files for trace_rawTransaction

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
                PR <a href="https://github.com/hyperledger/besu/pull/3443" class=".btn">#3443</a>
            </td>
            <td>
                <b>
                    QBFT Migration: allow active mining coordinator to be shutdown (with coverage)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">consensus</span>
            </td>
            <td>
                A better tested but more complex version of the solution from https://github.com/hyperledger/besu/pull/3438.

Pulled code apart to get decent unit test coverage.

https://github.com/hyperledger/besu/issues/3003

Signed-off-by: Simon Dudley <simon.dudley@consensys.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 06:16:11 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3439" class=".btn">#3439</a>
            </td>
            <td>
                <b>
                    Merge main into merge branch
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

Merge main into merge:
* latest circle-ci updates  (reason for this merge)
* trace_call

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 00:48:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3438" class=".btn">#3438</a>
            </td>
            <td>
                <b>
                    (removed assertions) QBFT Migration: allow active mining coordinator to be shutdown
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">consensus</span>
            </td>
            <td>
                Simple solution with async tasks but not easily testable. Compromised the unit tests in favour of simplicity/readability, given that the migration happy path will also be covered by acceptance tests.

This draft can be compared with https://github.com/hyperledger/besu/pull/3443 which compromises simplicity/readability for the sake of better unit tests.

https://github.com/hyperledger/besu/issues/3003

Signed-off-by: Simon Dudley <simon.dudley@consensys.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 22:54:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3437" class=".btn">#3437</a>
            </td>
            <td>
                <b>
                    forkchoiceUpdated implement kiln/1.0-alpha6 execution spec 
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
* address merge-at-genesis case for terminal-proof-of-work checks
* update forkchoice status field json to reflect kiln spec
* use `INVALID` responses according to spec rather than rpc errors (HTTP 400)
* return a result from forkchoiceUpdated rather than void return with exceptions
* unit tests and mock fixes for existing tests

https://github.com/ethereum/execution-apis/blob/v1.0.0-alpha.6/src/engine/specification.md

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3385 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 19:53:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3436" class=".btn">#3436</a>
            </td>
            <td>
                <b>
                    Quick workaround, to make acceptance tests to use a dynamic port for …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …engine rpc

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
        Created At 2022-02-15 15:16:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3434" class=".btn">#3434</a>
            </td>
            <td>
                <b>
                    Fixed stateDiff for trace_call and added tests for it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

There was a problem with the stateDiff generation of the `trace_call` API. In order to create the stateDiff the world updater always needs a parent. This was not ensured before. Because the tests were missing it was not caught in the CI pipeline. This PR fixes the issue for stateDiff and adds the tests for it as well.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 15:05:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3433" class=".btn">#3433</a>
            </td>
            <td>
                <b>
                    Altered empty header download handling.
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
Changed header downloading to write a log entry instead of throwing multiple exceptions when the header list is empty.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Addresses #3336 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 13:11:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3432" class=".btn">#3432</a>
            </td>
            <td>
                <b>
                    Persist last finalized block hash, prerequisite for The Merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rename CONSTANTS_PREFIX to VARIABLES_PREFIX,
since values stored there are not fixed and change over time.

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2913

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 11:46:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3431" class=".btn">#3431</a>
            </td>
            <td>
                <b>
                    move quorum ATs to nightly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Move Quorum ATs step to nightly. (These tests run Besu in GoQuorum privacy compatibility mode, with Tessera and EthSigner. So basically testing the same calls sent to GoQuorum work when sent to Besu)

Justification:
* tests are flaky, introducing noise into besu PR builds
* no regressions have been found since these tests were instated
* the downside is it may take longer to find a regression 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 08:49:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3430" class=".btn">#3430</a>
            </td>
            <td>
                <b>
                    CI nightly - skip test.sh in docker dir
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

When doing dockerScan step, skip the file named test.sh
Fixes #3426 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 06:37:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3429" class=".btn">#3429</a>
            </td>
            <td>
                <b>
                    RocketChat -> Discord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Replace Rocket Chat links with Discord. Reworded some links.

This does remove the badge from the top of the README. Requires Discord admin to setup if we want the equivalent for Discord. https://shields.io/category/chat

Fixes #3428 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 04:47:43 +0000 UTC
    </div>
</div>

