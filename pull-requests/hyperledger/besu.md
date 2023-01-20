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
                PR <a href="https://github.com/hyperledger/besu/pull/4969" class=".btn">#4969</a>
            </td>
            <td>
                <b>
                    Add withdrawals details to eth_getBlock methods
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

This is the critical piece that will allow Withdrawals interop to work.

Integration tests and any other RPCs that return a block will be added in a subsequent PR.

Signed-off-by: Simon Dudley <simon.dudley@consensys.net>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Critical piece of #4808

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-20 03:18:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4968" class=".btn">#4968</a>
            </td>
            <td>
                <b>
                    Withdrawals wiring
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
Final piece to wire together withdrawals and adding missing pieces

- withdrawalsRoot calculation
- withdrawals block body RLP encoding
- add withdrawalsRoot and withdrawals when creating a block
- validate withdrawals when validating mainnet blocks
- fix invalid withdrawals root during backwards sync
- include withdrawalsRoot when creating new header in EngineNewPayload

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-20 02:17:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4967" class=".btn">#4967</a>
            </td>
            <td>
                <b>
                    Change JSON RPC Error-32602 (Invalid Params) to return with http status code 200
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
This PR changes the JsonRpc http service to return the error -32602 (Invalid params) with a 200 http status code.  

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-20 01:51:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4965" class=".btn">#4965</a>
            </td>
            <td>
                <b>
                    Add a new CLI option to limit the number of requests in a single RPC batch request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Adds a `--rpc-max-batch-size` CLI option to restrict the maximum number of requests in a single RPC batch request.

Default `50`
When `-1`: unlimited - the current configuration.

When number of requests in batch > `--rpc-max-batch-size`:

- Throw a JsonRpcError.EXCEEDS_RPC_MAX_BATCH_SIZE; with type `INVALID_PARAM` and message `Number of requests in batch exceeds --rpc-max-batch-size.`

## Fixed Issue(s)
fixes #4951

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 16:37:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4964" class=".btn">#4964</a>
            </td>
            <td>
                <b>
                    Fix transaction pool issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description


There has been a regression on Besu regarding the transaction pool. Indeed it seems that the transaction pool validation part does not make a copy of the worldstate during the GetMutable and this means that we can have a version which can change and which is not safe. A copy mechanism has been set up which allows to use the snapshot and to protect against worldstate modifications during validation. it was used elsewhere except in transaction pool validation and block replay.

This caused us to invalidate too many transactions

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 14:16:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4963" class=".btn">#4963</a>
            </td>
            <td>
                <b>
                    Exclude Dagger generated sources from ErrorProne
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

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 13:38:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4962" class=".btn">#4962</a>
            </td>
            <td>
                <b>
                    Add withdrawals root to block header
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add the withdrawalsRoot to the block header.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 03:27:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4960" class=".btn">#4960</a>
            </td>
            <td>
                <b>
                    Layered Transaction Pool
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

WIP still not readt for review

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 18:28:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4959" class=".btn">#4959</a>
            </td>
            <td>
                <b>
                    Enforce EOF version validation rules
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

Add enforcement of the rule that EOF cannot create prior versions or legacy EVM code contracts in create opcodes and create transactions.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 15:51:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4958" class=".btn">#4958</a>
            </td>
            <td>
                <b>
                    New excess_data_gas block header field
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

Add `excess_data_gas` field to block header as for EIP-4844 specification

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 14:55:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4957" class=".btn">#4957</a>
            </td>
            <td>
                <b>
                    Updated overview builder to consider networkId and custom network genesis.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span>
            </td>
            <td>
                Signed-off-by: mark-terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Enhances the Configuration Overview to include networkId and custom genesis files (when specified.)

## Fixed Issue(s)
Fixes #4880 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 14:36:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4956" class=".btn">#4956</a>
            </td>
            <td>
                <b>
                    Add wcgcyx as maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Proposing @wcgcyx as a new Besu maintainer. They have made over 5 significant [commits](https://github.com/hyperledger/besu/pulls?q=is%3Apr+author%3Awcgcyx+is%3Aclosed) that have improved the quality of Besu and/or added new features.

Voting ends 2 weeks from the publication of this PR or once more than 50% of the current maintainers approve.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 07:27:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4955" class=".btn">#4955</a>
            </td>
            <td>
                <b>
                    Change BlockBody to use an overloaded constructor with withdrawals
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
Change BlockBody to use an overloaded constructor with withdrawals instead having a mandatory `Optional<List<Withdrawals>>` as withdrawals are only required for ethereum mainnet.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 06:26:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4954" class=".btn">#4954</a>
            </td>
            <td>
                <b>
                    Fix npe from subcommands
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
This fixes the NPE from some of the engine-api hive test that call the importBlock subcommand

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 04:37:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4953" class=".btn">#4953</a>
            </td>
            <td>
                <b>
                    engine_getPayloadV2 Withdrawals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Return withdrawals to engine_getPayloadV2, if they exist (implying it's a Shanghai block)

Spec: https://github.com/ethereum/execution-apis/blob/main/src/engine/shanghai.md#response-2

Also small unrelated fix to BlockReplay for Shanghai

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Fixes #4776
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 04:20:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4950" class=".btn">#4950</a>
            </td>
            <td>
                <b>
                    reduce hash address computation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 10:36:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4948" class=".btn">#4948</a>
            </td>
            <td>
                <b>
                    Fix TOML parsing of double and float values
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix TOML parsing of double 
- no special processing required for double or float
- refactor getInteger to getNumeric since it works for all number types
- added a test to ensure we can parse an int value into double type
eg 
tx-pool-limit-by-account-percentage=1.0
should work the same as
tx-pool-limit-by-account-percentage=1

Ref #4899 which didn't quite work for me. 
@bl0up does this work for you? 

Fixes #4896 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 05:49:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4947" class=".btn">#4947</a>
            </td>
            <td>
                <b>
                    Fix: Hive engine api FCU regression
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Swap lines order to ensure we commit FCU even if payload timestamp is before head timestamp

Signed-off-by: Gabriel Fukushima <gabrielfukushima@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR fixes the regression introduced recently.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Makes Besu compliant with ForkChoiceUpdate_V1 - item 7 of the Engine API specs for Paris. (https://github.com/ethereum/execution-apis/blob/main/src/engine/paris.md)

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 05:07:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4946" class=".btn">#4946</a>
            </td>
            <td>
                <b>
                    Implement engine_newPayload Withdrawals validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Spec: https://github.com/ethereum/execution-apis/blob/main/src/engine/shanghai.md

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Part of https://github.com/hyperledger/besu/issues/4776

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 03:54:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4945" class=".btn">#4945</a>
            </td>
            <td>
                <b>
                    Shanghai Engine API Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Zhenyang Shi <wcgcyx@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Update engine API to include some new changes introduced in 
- [ethereum/execution-apis#338](https://github.com/ethereum/execution-apis/pull/338) and 
- [ethereum/execution-apis#337](https://github.com/ethereum/execution-apis/pull/337)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4916 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 02:17:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4944" class=".btn">#4944</a>
            </td>
            <td>
                <b>
                    Add optional list of withdrawals to block body
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Signed-off-by: Jason Frame <jason.frame@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add optional list of withdrawals to block body. Also update the equals, hashcode methods. This does not wire withdrawals into the block body it's just to reduce the noise as many uses especially tests will use Optional.empty for withdrawals. Changes to wire in the list of withdrawals will be done in a subsequent PR.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 00:34:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4943" class=".btn">#4943</a>
            </td>
            <td>
                <b>
                    Remove noop WithdrawalsProcessor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Signed-off-by: Jason Frame <jason.frame@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Some cleanup, the noop withdrawals processor is no longer needed since ProtocolSpec returns an Optional<WithdrawalsProcessor> instead.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 00:05:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4942" class=".btn">#4942</a>
            </td>
            <td>
                <b>
                    Add implementation for eth_createAccessList RPC method 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span><span class="chip">TeamRevenant</span><span class="chip">mainnet</span><span class="chip">RPC</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

### Description

Missing implementation for eth_createAccessList rpc method

### Acceptance Criteria
- https://web3js.readthedocs.io/en/v1.7.0/web3-eth-contract.html#methods-mymethod-createaccesslist

This PR fixes the following failing test cases:

- https://github.com/ethereum/execution-apis/tree/main/tests/eth_createAccessList
  - eth_createAccessList/create-al-multiple-reads (besu)
  - eth_createAccessList/create-al-simple-contract (besu)
  - eth_createAccessList/create-al-simple-transfer (besu)

**Expected behavior:**
To return properties to be compatible with web3.

**Actual behavior:**
```
curl --data '{"method":"eth_createAccessList","params":[{"from": "0x8cd02c6cbd8375b39b06577f8d50c51d86e8d5cd", "data": "0x608060806080608155"}, "pending"],"id":1,"jsonrpc":"2.0"}' -H "Content-Type: application/json" -X POST localhost:8545
{
  "jsonrpc" : "2.0",
  "id" : 1,
  "error" : {
    "code" : -32601,
    "message" : "Method not found"
  }
}%  
```

## Fixed Issue(s)
#3400

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 18:22:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4940" class=".btn">#4940</a>
            </td>
            <td>
                <b>
                    Send only hash announcement for blob transaction type
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

When broadcasting transactions to peers, handle 4844 blob transactions in the following ways:

- For pre-eth/65 peers 4844 blob transactions are ignore are not sent
- For eth/65+ peers selected for full transaction body broadcast, a mixed approach is taken, and 2 messages are sent:
  - non-blob transactions are sent in full as before
  - for 4844 blob transactions only the hash is announced
- For eth/65+ peers selected for hash only announcements, same strategy as before, for all transactions (including 4844 blob ones) only the hashes are announced

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

implements #4821

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 13:10:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4939" class=".btn">#4939</a>
            </td>
            <td>
                <b>
                    Introduce transaction pool interface
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

Preparatory work to introduce more implementations of the transaction pool, specifically the new transaction pool that will support 4844.

No functionality changes in this PR, apart the introduction of the interface, sorter unit tests have been moved to the package of the corresponding classes

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 10:53:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4938" class=".btn">#4938</a>
            </td>
            <td>
                <b>
                    Improve get protocol schedule (only get header and not the entire block)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">performance</span><span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Karim TAAM [karim.t2am@gmail.com](mailto:karim.t2am@gmail.com)
Co-authored-by: Ameziane H [ameziane.hamlat@consensys.net](mailto:ameziane.hamlat@consensys.net)

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
There is a performance regression in the RC version 23.1.0-RC1 compared to 22.10.3 in both engine_getPayloadV1 and engine_forkchoiceUpdatedV1 calls. This regression is related to recent changes in the way we get the protocol specifications. We get the whole block by decoding each single transaction to use only the block header.
```
return Optional.ofNullable(protocolContext)
        .map(ProtocolContext::getBlockchain)
        .flatMap(blockchain -> blockchain.getBlockByNumber(number))
        .map(Block::getHeader)
        .map(timestampSchedule::getByBlockHeader)
        .orElseGet(
            () ->
                transitionUtils.dispatchFunctionAccordingToMergeState(
                    protocolSchedule -> protocolSchedule.getByBlockNumber(number)));
```

![image](https://user-images.githubusercontent.com/5099602/212659020-cd0c50d1-894c-423d-831c-ae8ff2b0784b.png)

The fix here is to use         
```.flatMap(blockchain -> blockchain.getBlockHeader(number))```

instead of
```  
.flatMap(blockchain -> blockchain.getBlockByNumber(number))
        .map(Block::getHeader)
```

Profiling on version 23.1.0-RC1 (with the regression)
![Screenshot 2023-01-16 at 11 18 31](https://user-images.githubusercontent.com/5099602/212657155-adbd67c8-a5e7-4b44-b23d-8fbd187096ee.png)


Profiling on version 22.10.3 (without the performance regression)

![image](https://user-images.githubusercontent.com/5099602/212658097-9db79cc5-5de7-41c4-a65c-aa6cd629ace5.png)

Block processing and FCU time

![image](https://user-images.githubusercontent.com/5099602/212666583-7b8c9704-87d9-4e60-803f-9564ff3dd89d.png)


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 09:33:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4937" class=".btn">#4937</a>
            </td>
            <td>
                <b>
                    [MINOR] fixed test for absent deprecated tx-pool-future-max-by-account
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <macfarla.github@gmail.com>

Fixes #4910 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 07:47:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4936" class=".btn">#4936</a>
            </td>
            <td>
                <b>
                    [MINOR] Correct order of args to RequestBody.create
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">dev experience</span>
            </td>
            <td>
                Content type moved to second arg where needed to avoid deprecation warning

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 07:21:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4935" class=".btn">#4935</a>
            </td>
            <td>
                <b>
                    Withdrawls - Change Amount type to GWei instead of Wei
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Withdrawls - Change Amount type to GWei instead of Wei

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4920 
https://github.com/ethereum/execution-apis/pull/354

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 06:06:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4933" class=".btn">#4933</a>
            </td>
            <td>
                <b>
                    Datahash opcode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Don't merge till https://github.com/hyperledger/besu/pull/4931/files has been merged.




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-15 21:31:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4932" class=".btn">#4932</a>
            </td>
            <td>
                <b>
                    doubled memory requirements for building
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-15 16:10:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4931" class=".btn">#4931</a>
            </td>
            <td>
                <b>
                    4844 new tx type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds the new enumeration for the 4844 blob data transaction type, and fixes many tests which surprisingly broke due to that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-15 16:02:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4930" class=".btn">#4930</a>
            </td>
            <td>
                <b>
                    fixes test that won't pass if local hostname unresolvable via reverse…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                … dns

Signed-off-by: Justin Florentine <justin+github@florentine.us>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-15 15:37:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4929" class=".btn">#4929</a>
            </td>
            <td>
                <b>
                    withdrawals-devnet-2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a record of what's currently running on withdrawals-devnet-2 (built from #4818) before I start changing what's on #4818 for the next devnet.

It's a combination of the following:

- shanghaiTimestamp https://github.com/hyperledger/besu/pull/4743
- WIP Withdrawals https://github.com/hyperledger/besu/pull/4552
(actually based this branch off the previously merged https://github.com/hyperledger/besu/pull/4758 and pulled in the recent shanghaiTimestamp changes)
- ForkId timestamp support https://github.com/hyperledger/besu/pull/4815
- EIP-3651 Warm COINBASE - wiring: https://github.com/hyperledger/besu/pull/4818/commits/682fb7f3b42c07c2bee404d9466d0e17e1b1ea18
- EIP-3855 PUSH0 - wiring: https://github.com/hyperledger/besu/pull/4818/commits/a47cce61f5ca4a78b407d1c3a353bd09085fa4d6
- EIP-3860 Limit/meter initcode - wiring: https://github.com/hyperledger/besu/pull/4818/commits/36add0782d70375a7a42a4bd57dbca0b5f8cd0ab
- Add blockValue to engine_getPayloadV2: https://github.com/hyperledger/besu/pull/4833 (https://github.com/ethereum/execution-apis/pull/314)
- Add withdrawals to getBlockByHash and getBlockByNumber: https://github.com/hyperledger/besu/pull/4818/commits/161b70c74b06f94a4722b983aded45811364332a (https://github.com/ethereum/execution-apis/pull/334)
- withdrawals-devnet-1 fixes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-14 21:25:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4928" class=".btn">#4928</a>
            </td>
            <td>
                <b>
                    fixes test that won't pass if local hostname unresolvable via reverse…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                … dns

Signed-off-by: Justin Florentine <justin+github@florentine.us>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-14 18:41:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4927" class=".btn">#4927</a>
            </td>
            <td>
                <b>
                    Cherry pick burn-in release 22.10.4
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
Cherry picks include:

* b4e2cdb82 2022-12-21 | Use safe block as pivot block suring snapsync (#4819) [matkt]
* 418d392fa 2022-12-22 | Bugfix snapshot transaction segfaults after storage truncation (#4786) [garyschulte]
* adb76c597 2022-12-23 | Bugfix potential chain head and worldstate inconsistency (#4862) [garyschulte]
* 33ee2bba6 2023-01-08 | Peering - disconnect worst peer (#4888) [Sally MacFarlane]
* b4d5e9d27 2023-01-11 | Attempt to fix CPU spikes issue (#4867) [ahamlat]
* bc4f9e7a7 2023-01-12 | not block subscribe when the worldstate storage is open (#4912) [matkt]
* a5e3ed4f4 2023-01-13 | Address bonsai self-destruct stale code present  (#4906) (HEAD -> cherry-pick-22.10.4, 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-14 01:16:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4926" class=".btn">#4926</a>
            </td>
            <td>
                <b>
                    Update 22.10.x
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
bring release-22.10.x branch up to 22.10.3

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-14 00:36:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4925" class=".btn">#4925</a>
            </td>
            <td>
                <b>
                    Bonsai consistency check startup subcommand
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
Adds a besu subcommand which will check and attempt to fix bonsai inconsistencies between the chain head and worldstate head.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-14 00:07:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4924" class=".btn">#4924</a>
            </td>
            <td>
                <b>
                    Optimization for eth_call use of blockHeader <> hash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Optimization for eth_call 
* previously was getting header, getting blockHash, creating ChainHead with hash, and then getting header by hash again - and under load, sometimes, was getting null for the header by hash - even though we know there is a header because that's how we got the hash in the first place. This is what caused the occasional 'block not found' errors per #4192 
* refactor to store the header on ChainHead and get the hash when needed

Fixes #4192 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 22:57:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4919" class=".btn">#4919</a>
            </td>
            <td>
                <b>
                    Adding preliminary SSZ encoding/decoding of Transaction Network Payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 16:19:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4918" class=".btn">#4918</a>
            </td>
            <td>
                <b>
                    improve preload cache
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

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 13:56:58 +0000 UTC
    </div>
</div>

