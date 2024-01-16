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
                PR <a href="https://github.com/hyperledger/besu/pull/6413" class=".btn">#6413</a>
            </td>
            <td>
                <b>
                    IGNORE - trie log pruner test
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
        Created At 2024-01-16 04:42:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6412" class=".btn">#6412</a>
            </td>
            <td>
                <b>
                    [CI] publish tasks don't depend on test tasks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                occasional flakiness eg https://app.circleci.com/pipelines/gh/hyperledger/besu/26365/workflows/c1646864-be7d-4a67-95dc-ab22876dbdde should not stop publish tasks

all required test tasks have already passed on PR runs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-16 03:54:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6411" class=".btn">#6411</a>
            </td>
            <td>
                <b>
                    Remove  deprecated `--privacy-onchain-groups-enabled` option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">privacy</span><span class="chip">doc-change-required</span><span class="chip">non mainnet (private networks)</span>
            </td>
            <td>
                ## PR description
Remove  deprecated `--privacy-onchain-groups-enabled` option

## Fixed Issue(s)
fixes #6410 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-16 02:15:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6407" class=".btn">#6407</a>
            </td>
            <td>
                <b>
                    Allow Xpoa-block-txs-selection-max-time to be greater than 100%
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

In #6044 `Xpoa-block-txs-selection-max-time` options has been introduced to limit the block creation time to a fraction of the genesis block time, but there are cases where it is useful to let the block creation time last more, so with this PR is it possible to specify value greater than 100%

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 11:04:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6406" class=".btn">#6406</a>
            </td>
            <td>
                <b>
                    cliqueBft AT task flakiness - extend no_output_timeout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                task is flaky eg 20 min with no response https://app.circleci.com/pipelines/github/hyperledger/besu/26348/workflows/3c01f02c-3127-4b9c-965f-a869096ef3a5/jobs/173374 and https://app.circleci.com/pipelines/github/hyperledger/besu/26350/workflows/1c5f785f-f62b-4fa7-97cf-097dde63325c/jobs/173389

increase `no_output_timeout` to 30min

~~reverts #6392 - seems to have caused flakiness~~ 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 07:02:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6405" class=".btn">#6405</a>
            </td>
            <td>
                <b>
                    remove X flag from SNAP sync mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                refs #6311 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 04:38:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6404" class=".btn">#6404</a>
            </td>
            <td>
                <b>
                    Bonsai keyvalue refactor
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
Refactor `BonsaiWorldStateKeyValueStorage` to move the FlatDB construction and management out into a new class `FlatDbStrategyProvider`.

- Splits out the FlatDbStrategy construction and flatDb management from the BonsaiWorldStateKeyValueStorage into a new class FlatDbStrategyProvider
- Passes through the DataStorageConfiguration to FlatDbStrategyProvider instead of just the boolean flag

By splitting out the FlatDbStrategy I can simplify the constructor arguments to the BonsaiWorldStateKeyValueStorage quite a bit as I can create the FlatDbStrategyProvider in the KeyValueStorageProvider once with its arguments instead of repassing those into the BonsaiWorldStateKeyValueStorage each time we create an instance of it.

Note: The DataStorageConfiguration parameter isn't used in the FlatDbStrategyProvider but will be used in a subsequent PR to add the code storage by code hash functionality.

### Testing
- Checkpoint sync on Goerli

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 03:08:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6403" class=".btn">#6403</a>
            </td>
            <td>
                <b>
                    Snap sync downloader logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * use non-static logger field so that SnapSyncDownloader will own the logging lines
   * Note this is a departure from the standard Logger field used elsewhere in the codebase. However it is flagged by the annotation so it's obvious. Couldn't think of a nicer way to do this but open to suggestions
* rename SnapsyncMetricsManager to SnapSync... for consistency
* rename FastImportBlockStep to ImportBlockStep
* rename SyncTargetManager to AbstractSyncTargetManager and FastSyncTargetManager to SyncTargetManager
* rename FastSyncException to SyncException

fixes #6386 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 01:24:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6401" class=".btn">#6401</a>
            </td>
            <td>
                <b>
                    log a different warning if pruning is enabled with BONSAI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                log "ignored" if enabled with BONSAI vs "deprecated" if enabled with FOREST

fixes #6400
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-14 21:50:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6397" class=".btn">#6397</a>
            </td>
            <td>
                <b>
                    Upgrade Mockito
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

Upgrade Mockito to 5.8.0, that is a breaking change, and requires some code changes, in particular to avoid spying on maps.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-12 17:59:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6396" class=".btn">#6396</a>
            </td>
            <td>
                <b>
                    Upgrade Guava dependency
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

Upgrade Guava to 33.0.0, since it introduces a change in the Supplier class, the memory consumption estimation of a pending transaction has been updated to take in account the new layout of the class.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-12 11:16:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6395" class=".btn">#6395</a>
            </td>
            <td>
                <b>
                    Fix typo in SUPPORT.md
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

fix `Hyperlegder` to `Hyperledger`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-12 08:29:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6394" class=".btn">#6394</a>
            </td>
            <td>
                <b>
                    Trie log prune using TrieLogEvent
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
This PR aims to make the pruning logic async as this feature does not need to be in the synchronous.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Part of #5390 

## Testing

Tested locally on a small chain.
Will bundle canary testing with some other PRs as part of getting this feature production ready, see task list for #5390
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-12 07:50:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6392" class=".btn">#6392</a>
            </td>
            <td>
                <b>
                    reduce machine size for clique/BFT ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                same change as was made in #6384 for permissioning ATs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-12 04:26:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6390" class=".btn">#6390</a>
            </td>
            <td>
                <b>
                    Use mining beneficiary from protocol spec in TraceServiceImpl
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

instead of using coinbase from block header as mining beneficiary, we use the protocol spec to retrieve it

## Fixed Issue(s)
fixes #6389 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-11 23:53:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6387" class=".btn">#6387</a>
            </td>
            <td>
                <b>
                    [MINOR] Fix pki tests condition check on mac
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix pki tests condition check on mac

## Fixed Issue(s)
see https://github.com/hyperledger/besu/pull/6235
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-11 02:25:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6384" class=".btn">#6384</a>
            </td>
            <td>
                <b>
                    Fix test flackyness of acceptanceTestsPermissioning 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">flake</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

`NodeSmartContractPermissioningAcceptanceTest` could fail due to the fact that if a node is not in sync txs are not accepted, since the txpool is disabled, so before interacting with the node we must wait for all the nodes in the test to be in sync.
Also tuned Circle CI to execute acceptanceTestsPermissioning serially, to avoid to spawn too many Besu processes and in that way it is enough to use a medium executor, as last thing slowed a bit the block creation to make synchronization easier.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 20:57:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6383" class=".btn">#6383</a>
            </td>
            <td>
                <b>
                    Bump to nex release snapshot 24.1.1
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
bump release version to 24.1.1-SNAPSHOT
add/edit/move changelog entries
TBA links for 24.1.0
add missing changelog entry for 23.10.2

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 18:29:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6382" class=".btn">#6382</a>
            </td>
            <td>
                <b>
                    In fluent APIs correct Tangerine Whistle definition.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The fluent API incorrectly added the code size limit in Tangerine Whistle instead of first adding it in Spurious Dragon.

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
        Created At 2024-01-10 18:14:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6381" class=".btn">#6381</a>
            </td>
            <td>
                <b>
                    Introduce TransactionEvaluationContext to pass data between selectors and plugin
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

Some tx selector plugins needs more context about the current tx being evaluated, for example the current minGasPrice, or the effective price of the tx and possibly more data in the future, for this we introduce the TransactionEvaluationContext to hold that data and pass it across all the selectors and the plugin. Another advantage of this context is to avoid to compute multiple time the same data, in case it is needed in more that one selector.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 13:15:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6380" class=".btn">#6380</a>
            </td>
            <td>
                <b>
                    Make transaction pool configurable in acceptance tests
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
        Created At 2024-01-10 13:10:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6379" class=".btn">#6379</a>
            </td>
            <td>
                <b>
                    Ignore bin files when running the spdx license check
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
Ignore generated files in `bin/` directories when running the SPDX license check.  Visual Studio Code generates build files in various bin directories, which causes this check to fail.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 21:29:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6378" class=".btn">#6378</a>
            </td>
            <td>
                <b>
                    Upgrade `com.fasterxml.jackson` dependencies
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

Jackson 2.15 by default limits the length of input string to a value that is lower than the string length used in some of our test, so now we need to explicitly tune this value. Setting max int since this is only related to tests. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 15:56:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6377" class=".btn">#6377</a>
            </td>
            <td>
                <b>
                    Upgrade dependencies
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

Update all dependencies that do not require code changes.

Dependencies that require code changes will be updated in separate PR.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 12:57:54 +0000 UTC
    </div>
</div>

