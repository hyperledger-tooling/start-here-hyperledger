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
                PR <a href="https://github.com/hyperledger/besu/pull/5968" class=".btn">#5968</a>
            </td>
            <td>
                <b>
                    Issue 5544 - Tessera as internal process
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
Fixes #5544 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 11:59:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5967" class=".btn">#5967</a>
            </td>
            <td>
                <b>
                    [4844] FCU Validate badblock before sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Validate bad blocks before asking for a new sync
## Fixed Issue(s)
fixes #5950
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 10:35:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5966" class=".btn">#5966</a>
            </td>
            <td>
                <b>
                    Use PendingTransaction in BlockTransactionSelector
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

This is just a refactoring, no functionality change, to have the `PendingTransaction` object during the selection of transactions, since in the `PendingTransaction` there are additional metadata about the candidate transaction that can be used by the selection process, and more will be added in a next PR to better support priority senders.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 09:08:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5964" class=".btn">#5964</a>
            </td>
            <td>
                <b>
                    add plugins summary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                log a summary of plugins at registration time
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 01:55:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5961" class=".btn">#5961</a>
            </td>
            <td>
                <b>
                    Apply fcu even on invalid payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes more Hive tests when a payload that is invalid is passed along with an FCU
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 00:11:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5960" class=".btn">#5960</a>
            </td>
            <td>
                <b>
                    Optionally bypass state root verification in reference test worldstate
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
if the passed block header has a stateroot of Hash.ZERO, bypass bonsai state root verification in bonsai reference test worldstate only.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5934 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 20:45:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5959" class=".btn">#5959</a>
            </td>
            <td>
                <b>
                    Priority senders
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

This PR is build on top of #5966 so please check it first. [Relative diff](https://github.com/fab-10/besu/compare/main...priority-senders)

This PR expand the concept of priority of txs and senders. Currently in Besu by default every tx sent using the RPC API is called _local_, and _local_ is also a synonym for _priority_, that means that the tx does not need to satisfy the min price option and it is selected first when building a block, the txs received via p2p are called _remote_ and haven't any priority.
It is possible to disable this default behavior passing the option `--tx-pool-disable-locals`, and all txs are treated the same.
This simple approach does not works well if Besu is used as a gateway to publish txs for multiple senders, when the node owner what to prioritize only a subset of them, to support this use case, this PR add the `--tx-pool-priority-senders` option, with it is possible to specify the list of senders, whom txs have priority, regardless their origin, both local or remote.

Since _local_ is not always synonym of _priority_, the concepts have been separated, and so a `PendingTransaction` has both attributes as distinct fields, where _local_ is now only used to identify the source and _priority_ is used to apply or not the min price option and during the selection when building a block. To note that txs with priority will be dropped from the pool after the other ones.

To follow the new semantic of `--tx-pool-disable-locals` has been deprecated for removal in favor of `--tx-pool-no-local-priority`

To resume the possibility of mixing the priority options are:
1. Default (no option specified): All txs sent via RPC API are prioritized
2. `--tx-pool-no-local-priority=true`: No tx is prioritized
3. `--tx-pool-priority-senders=sender1,sender2`: All txs sent via RPC API are prioritized + all txs sent by _sender1_ and _sender2_
4. `--tx-pool-no-local-priority=true` `--tx-pool-priority-senders=sender1,sender2`: Only txs sent by _sender1_ and _sender2_ are prioritized

Regression tests in progress and will merge after they pass.

## Fixed Issue(s)
Partially fixes #5829 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 19:04:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5957" class=".btn">#5957</a>
            </td>
            <td>
                <b>
                    Added toString implementation for TransactionSimulatorResult
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
Added toString implementation for TransactionSimulatorResult

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fix #5942
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 09:45:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5955" class=".btn">#5955</a>
            </td>
            <td>
                <b>
                    rlpx - Send empty list instead of Empty Bytes for the Ping and Pong message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Send empty list instead of Empty Bytes for Ping and Pong message
https://github.com/ethereum/devp2p/blob/master/rlpx.md#ping-0x02
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 07:07:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5954" class=".btn">#5954</a>
            </td>
            <td>
                <b>
                    Fixup changelog following 23.7.3 release
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
        Created At 2023-09-27 05:03:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5953" class=".btn">#5953</a>
            </td>
            <td>
                <b>
                    Release 23.7.3
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
        Created At 2023-09-27 02:38:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5952" class=".btn">#5952</a>
            </td>
            <td>
                <b>
                    Update execution tests to 0.2.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #5412 

Number of ref tests 
* main - 185426: https://app.circleci.com/pipelines/github/hyperledger/besu/24196/workflows/ae4e3b27-f74d-4d04-83c8-d515a3da9b75/jobs/155337
* this PR - 185441: https://app.circleci.com/pipelines/github/hyperledger/besu/24197/workflows/a23689ff-a74c-494f-bfdb-650dc9fd61c9/jobs/155355
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 00:32:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5949" class=".btn">#5949</a>
            </td>
            <td>
                <b>
                    Forkchoice v2 hive tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                re-arranges validations so the failures occurr when hive expects them to.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-26 18:21:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5948" class=".btn">#5948</a>
            </td>
            <td>
                <b>
                    Transaction pool unit tests refactoring to remove duplicated code
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

Refactor transaction pool tests to remove all the duplicated code that was introduced when implementing the layered txpool.
Now all tests are defined in `AbstractTransactionPoolTest` and extending classes are used to setup the right env for fee market and txpool implementation.
This make the tests more future proof, since in this way a new test is run against all the implementations and fee markets, while before you had to remember to code the test twice.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-26 16:37:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5941" class=".btn">#5941</a>
            </td>
            <td>
                <b>
                    updated beacon root and modulus to match DRAFT eip
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Still draft but this time it _says_ final https://github.com/ethereum/EIPs/pull/7672#issuecomment-1734562996

Also renamed the modulus value so it matches the name used in the EIP
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-26 06:30:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5940" class=".btn">#5940</a>
            </td>
            <td>
                <b>
                    [4844] [Hive] Fix fcuV3 parameter return 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix some hive tests

- Return JsonRpcErrorResponse instead of JsonRpcSuccessResponse when fork not supported or parameters invalid.
- Validate parameter before fork validation
- Validate getParentBeaconBlockRoot on EngineForkchoiceUpdatedV3 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-26 02:34:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5939" class=".btn">#5939</a>
            </td>
            <td>
                <b>
                    Add Nick and George as maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I propose to add @nicksneo and @gtebrean as Besu project maintainers. In addition to quality code contributions, they have been contributing to Besu community via contributing to discussions in Discord. 

Nick has made a number of code contributions including -
* show correct revert reason data in priv_call
* removed GoQuorum permissioning interop
* migrated several packages from Junit4 to Junit5

Nick’s PRs: https://github.com/hyperledger/besu/pulls?q=is%3Apr+is%3Aclosed+author%3ANickSneo

George has made a number of code contributions including - 
* bugfix in eth_feeHistory
* decoupled JsonRPCError enum from the data field
* made pretty JSON feature user-configurable

George's PRs: https://github.com/hyperledger/besu/pulls?q=is%3Apr+is%3Aclosed+author%3Agtebrean

Voting ends two weeks from today.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-26 02:05:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5938" class=".btn">#5938</a>
            </td>
            <td>
                <b>
                    Release 23.7.3-RC2 - Holesky Hotfix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using https://github.com/hyperledger/besu/tree/release-23.7.x, revert RC1 burn-in and apply holesky 2.0 config update as a cherry-pick.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-26 01:02:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5936" class=".btn">#5936</a>
            </td>
            <td>
                <b>
                    Fix t8n encoding issue
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

When sending a stack in json fields strip out the newlines and tabs.


## Fixed Issue(s)
fixes #5910 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-25 21:28:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5933" class=".btn">#5933</a>
            </td>
            <td>
                <b>
                    Cache last blocks data (block headers, block bodies, transactions' receipts and total difficulty)
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
Cache last blocks data (block headers, block bodies, transactions' receipts and total difficulty).
The default number of blocks to keep in the cache is 512.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-25 09:19:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5931" class=".btn">#5931</a>
            </td>
            <td>
                <b>
                    BlockTransactionSelector refactoring
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
`BlockTransactionSelector` refactoring:

- Extract `TransactionSelectionResults` to its own class.
- Extract Transaction Selection Criteria and selection logic out of the `BlockTransactionSelector` to their own classes
- `BlockTransactionSelector` will use a list of selectors to evaluate the transaction
- Similar to selectors that will evaluate a transaction

Next steps:

- Expose `TransactionProcessingResult` (or at least a part of it the to Plugin interface)
- Abstract the transaction selectors and external transaction selectors so they share the same logic
- Add a way to get the `OperationTracer` from the TPR and pass it to the plugin 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-25 03:22:42 +0000 UTC
    </div>
</div>

