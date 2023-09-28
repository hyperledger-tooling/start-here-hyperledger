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
                PR <a href="https://github.com/hyperledger/besu/pull/5963" class=".btn">#5963</a>
            </td>
            <td>
                <b>
                    allow BLOB txs during shanghai
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                covers first block after the fork case, merge after #5961 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 01:38:02 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5930" class=".btn">#5930</a>
            </td>
            <td>
                <b>
                    Add parameters to EVM library fluent API
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

Add the ability to configure more parameters in the fluent API. Specifically contract address, coinbase, difficulty, mixHash/prevRandao, baseFee, block number, timestamp, gas limit, previous block hashes, and versioned hashes.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-22 15:28:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5929" class=".btn">#5929</a>
            </td>
            <td>
                <b>
                    [4844] Fix some Devnet9 Hive tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix null latest valid hash when validation blobs/expected hashes
Fix HISTORICAL_ROOTS_MODULUS used by hive/devnet 9
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-22 07:45:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5923" class=".btn">#5923</a>
            </td>
            <td>
                <b>
                    Add Cancun GraphQL fields
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

Add the fields for Blobs into the GraphQL service.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 17:31:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5921" class=".btn">#5921</a>
            </td>
            <td>
                <b>
                    Always enforce promotion filter for transactions in the prioritized layer
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

This PR is built on top of #5920, so please check it first ([relative changes](https://github.com/fab-10/besu/compare/fab-10:besu:txpool-promotion-performance...prioritized-promotion-filter2))

This PR is preparatory for more work on prioritizing local txs, that consist in more small PRs that have been split to make it easier to review.
Before the PR, the prioritized layer also kept txs that could not be selected to be included in the next block, because as far as there was still space txs were added and kept there, regardless they were or not satisfying the promotion filter anymore.
This PR improves the content of the prioritized layer, keeping there only txs that always satisfy the promotion filter, and thus are candidate for inclusion in the next block, this avoid to waste some work during txs selection, and pave the way for an easier prioritization of local txs.
Currently the promotion filter says that a tx is willing to pay at list the base fee, on base fee market network, otherwise is always true.

Simulation of block production shows no regression, actually metrics about number of txs in the block, block value and gas used are, on average, better with this PR vs 23,7,2 version:
![image](https://github.com/hyperledger/besu/assets/91944855/309a58ac-838e-4da6-b3e7-703b9ce5644b)

![image](https://github.com/hyperledger/besu/assets/91944855/3a019711-770c-4d26-b1b7-7555d8ba2b71)

![image](https://github.com/hyperledger/besu/assets/91944855/ddad0bc1-9ece-4507-99f8-efa38a46db6a)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 16:35:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5920" class=".btn">#5920</a>
            </td>
            <td>
                <b>
                    Improve performance when promoting transaction from next layers
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

During the implementation of #5921, a performance issue surfaced in the way the promotion of transactions, from lower layers, was implemented.
The issue was that, to keep the code simple, the promotion was done for one tx at once, but with the improvement on the prioritized layer done #5921, this approach is no more practical since result in a quadratic complexity (number of confirmed txs per number of senders in the ready layer), so the solution is to do the promotion only once after all the confirmed txs have been processed, so the time is linear.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 16:33:52 +0000 UTC
    </div>
</div>

