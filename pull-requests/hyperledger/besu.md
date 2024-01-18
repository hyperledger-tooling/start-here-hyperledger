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
                PR <a href="https://github.com/hyperledger/besu/pull/6425" class=".btn">#6425</a>
            </td>
            <td>
                <b>
                    Fix to increment/decrement gas-limit in block production 
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
Fixes discord bug found by protoplanetary 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-18 02:25:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6423" class=".btn">#6423</a>
            </td>
            <td>
                <b>
                    Promote block txs selection max time options to stable
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

Promote block txs selection max time options to stable.
Both options were introduced in #6044, and are working fine since them, with the promotion the hard caps have been removed since that could be an issue with existing networks that are used to have longer block creation times.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 13:46:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6422" class=".btn">#6422</a>
            </td>
            <td>
                <b>
                    Upgrade prometheus
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
        Created At 2024-01-17 13:04:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6419" class=".btn">#6419</a>
            </td>
            <td>
                <b>
                    Downgrade rocksdbjni to 8.3.2 following FOREST bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bug introduced by upgrading to 8.9.1 in  [`9b7efb9` (#6377)](https://github.com/hyperledger/besu/pull/6377/commits/9b7efb9ed62789efd4f7d048d221871d73e50d9b)

This is a revert of that specific dependency, will need further work to fix FOREST + 8.9.1+

Tested on the canary that found the bug: prd-elc-besu-prysm-mainnet-nightly-forest-snap
and synced a fresh FOREST and BONSAI node on holesky.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 05:43:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6418" class=".btn">#6418</a>
            </td>
            <td>
                <b>
                    Addition of Profile Configuration CLI Option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">doc-change-required</span><span class="chip">ux</span>
            </td>
            <td>
                ## PR description
This pull request introduces the `--profile` CLI option to Besu. This new feature allows users to load existing TOML configuration files from resources, enabling the override of default options. This PR does not create the profiles - they will be created in different PRs.

- Profile CLI Option: The `--profile` CLI option has been added, providing users the ability to set the profile Besu should utilise for its configuration.

- Configuration Resolution: The configuration provider resolves settings in a cascading manner, prioritising environment variables, followed by the configuration file, the profile file (if any), and finally falling back to the variable default if no other configuration source is available.

For instance, consider a scenario where you have two TOML configuration files: `config.toml` and `staker.toml`. The `config.toml` file is provided by the user via the `--config-file` option, and `staker.toml` is a pre-configured resource file containing custom settings. The staker.toml file can be specified using the new --profile option:

`besu --config-file=config.toml --profile=STAKER`

In this case, Besu would first look for settings in the environment variables. If a setting is not found in the environment variables, Besu would look for it in the config.toml file. If the setting is not found in the config.toml file, Besu would then look for it in the `staker.toml` file. If the setting is not found in the `staker.toml` file, Besu would use the default value for that setting.

The rationale for using the TOML format to define profiles is as follows:

- It leverages existing TOML parsing and validation mechanisms
- The format is user-friendly
- It consolidates all configuration data into a single location

## Fixed Issue(s)
fixes #6323




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 05:06:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6417" class=".btn">#6417</a>
            </td>
            <td>
                <b>
                    Feature/reduce receipt size
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
Built on #5392 with the latest main changes merged in so can do testing on some nodes.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 00:31:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6415" class=".btn">#6415</a>
            </td>
            <td>
                <b>
                    use reference tests to verify trielog generation
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

This PR use reference tests to validate trielog generation. Like that we will validate our trielog generation for all of the tests we have in the references tests suite for past and future EIPs

I was able to validate that this PR can detect the issues we had before on mainnet by running this test "GeneralStateTests/stSStoreTest/InitCollision.json" with and without [the last ](https://github.com/hyperledger/besu/pull/6359) fix

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-16 16:11:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6414" class=".btn">#6414</a>
            </td>
            <td>
                <b>
                    Upgrade tech.pegasys.discovery:discovery
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
        Created At 2024-01-16 13:53:39 +0000 UTC
    </div>
</div>

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
                <span class="chip">privacy</span><span class="chip">non mainnet (private networks)</span>
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
                    SNAP and CHECKPOINT sync modes - now production ready
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * prefer SNAP and CHECKPOINT
* still support X_SNAP and X_CHECKPOINT - mark for deprecation in 24.4.0
* all help and log messages now use SNAP and CHECKPOINT

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
This refactors `BonsaiWorldStateKeyValueStorage` so it is easier to pass configuration into Bonsai and remove the need to pass in individual flags for features. I've moved the FlatDB construction and management out into a new class `FlatDbStrategyProvider` and this can be created just once and simplifies the creation of the `BonsaiWorldStateKeyValueStorage` with less args to be passed around each time it is created.

- Splits out the FlatDbStrategy construction and flatDb management from the BonsaiWorldStateKeyValueStorage into a new class FlatDbStrategyProvider
- Passes through the DataStorageConfiguration to FlatDbStrategyProvider instead of just the boolean flag

By splitting out the FlatDbStrategy I can simplify the constructor arguments to the BonsaiWorldStateKeyValueStorage quite a bit as I can create the FlatDbStrategyProvider in the KeyValueStorageProvider once with its arguments instead of repassing those into the BonsaiWorldStateKeyValueStorage each time we create an instance of it.

Note: The DataStorageConfiguration parameter isn't used in the FlatDbStrategyProvider but will be used in a subsequent PR to add the code storage by code hash functionality.

### Testing
- Checkpoint sync on Goerli
- Checkpoint sync on Mainnet
- Checkpoint sync with flat healing enabled on Goerli

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

