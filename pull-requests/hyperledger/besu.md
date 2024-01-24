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
                PR <a href="https://github.com/hyperledger/besu/pull/6455" class=".btn">#6455</a>
            </td>
            <td>
                <b>
                    ignore bws sync requests until initial sync is complete
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

Draft PR to verify impact of concurrent BWS on syncing nodes

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 23:07:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6453" class=".btn">#6453</a>
            </td>
            <td>
                <b>
                    feat: add `OperationTracer.tracePrepareTransaction`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

`OperationTracer.traceStartTransaction` is triggered before the EVM execution, but after the sender account has been updated (i.e. its balance decreased from the upfront cost and its nonce increased), hiding its actual initial state from the `OperationTracer`.

This PR adds a new hook, `OperationTracer.tracePrepareTransaction`, that is triggered after the transaction has been validated for execution, but before any change to the sender account, hence presenting its pristine state to the `OperationTracer`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 17:49:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6452" class=".btn">#6452</a>
            </td>
            <td>
                <b>
                    Feature/keccak impro
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
        Created At 2024-01-23 14:23:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6451" class=".btn">#6451</a>
            </td>
            <td>
                <b>
                    manage empty range for storage
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
        Created At 2024-01-23 14:22:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6449" class=".btn">#6449</a>
            </td>
            <td>
                <b>
                    Add selfish staker profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Add selfish staker profile

Use
`besu --profile=selfishstaker`

## Fixed Issue(s)
fixes https://github.com/hyperledger/besu/issues/6324
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 04:13:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6448" class=".btn">#6448</a>
            </td>
            <td>
                <b>
                    Add enterprise/private profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add enterprise/private profile 

Use:
`besu --profile=enterprise` or `besu --profile=private`

## Fixed Issue(s)
fixes #6326
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 03:55:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6446" class=".btn">#6446</a>
            </td>
            <td>
                <b>
                    Enable limit on range Of JSON-RPC API trace_filter method (#5971)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enable a limit on the range of blocks that can be supplied to the JSON-RPC trace_filter method.

The limit has a default value and can be overridden with a command line option at start up.

fixes #5971 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 21:27:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6445" class=".btn">#6445</a>
            </td>
            <td>
                <b>
                    Reuse --bonsai-historical-block-limit for limit trie logs feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Part of https://github.com/hyperledger/besu/issues/5390

* `$BESU --Xbonsai-limit-trie-logs-enabled=true` will use the default value of `--bonsai-historical-block-limit=512`
* `$BESU --Xbonsai-limit-trie-logs-enabled=true --bonsai-historical-block-limit=511` throws error as must be >= 512
* `$BESU --Xbonsai-limit-trie-logs-enabled=false --bonsai-historical-block-limit=511` does not throw error as this is allowed until limit-trie-logs-enabled.

This implementation avoids a breaking change for anyone that has a node with --bonsai-historical-block-limit already set to < 512 (could be noone?)

However, we should be aware that if `--Xbonsai-limit-trie-logs-enabled` ever becomes default then this breaking change will come back again
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 21:20:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6444" class=".btn">#6444</a>
            </td>
            <td>
                <b>
                    Fix `poa-block-txs-selection-max-time` option that was inadvertently reset to its default after being configured
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

Fix `poa-block-txs-selection-max-time` option that was inadvertently reset to its default after being configured.
Mining options needs the value of the block period from the genesis file, so the way to pass it to the class has been improved to avoid using the mining options if that value was not set, in order to be less error prone.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 14:58:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6443" class=".btn">#6443</a>
            </td>
            <td>
                <b>
                    Disconnect worst peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
In AbstractRetryingSwitchingPeerTask.java the method refreshPeers() we are now disconnecting the least useful peer. 
Another change is that now the peer table is refreshed until we have reached our maxPeers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 08:22:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6441" class=".btn">#6441</a>
            </td>
            <td>
                <b>
                    Ensure that Bonsai tests with Key Value storage are using Bonsai data configuration
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
Ensure that Bonsai tests with Key Value storage are using Bonsai data configuration. As these key-value storage are explicit with Bonsai classes this doesn't cause an issue using the default forest config but for readability, it is better to use the Bonsai data storage configuration.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 01:43:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6439" class=".btn">#6439</a>
            </td>
            <td>
                <b>
                    Only accept an address from a peer if it is a valid IP address
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
When using the `From` address specified by a peer, ensure it is a valid IP address. Otherwise revert to using the UDP source host.

## Fixed Issue(s)
See comment https://github.com/hyperledger/besu/pull/6225#issuecomment-1900243754
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-19 11:58:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6438" class=".btn">#6438</a>
            </td>
            <td>
                <b>
                    Fix changelog after incorrect merge of 6225
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
When https://github.com/hyperledger/besu/pull/6225 was updated with main before merging, the changelog entry remained in the old release
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-19 10:38:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6437" class=".btn">#6437</a>
            </td>
            <td>
                <b>
                    Log changes in BFT validators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
When the set of IBFT or QBFT validators changes between blocks, an `INFO` message is written listing the previous block number and its validators, as well as the pending block's number and validators.

This serves as a useful indicator that BFT voting has completed for a change in validators.

This log entry will not be written for public chain nodes so it should not introduce any unnecessary noise for public chain users. It isn't expected that validator changes in permissioned, BFT chains are likely to be so frequent that this log will be too noisy for those scenarios either.

I specifically didn't make it a `DEBUG` message since the validator list is key to how the BFT chain works, any changes to it are likely to be useful to an administrator/operator looking at just `INFO` logs, and as mentioned above these aren't expected to be very frequent.

Example output for a change from 1 validator node to 2 validator nodes:

```
2024-01-19 09:49:37.099+00:00 | main | INFO  | MessageValidatorFactory | Validator list change. Previous chain height 590245: [0x44740bDE71Ff5e8cd08c58a721A38Aaf62779478]. Current chain height 590246: [0x11427D85C111024762b0f6df9bfC575f4303F588, 0x44740bDE71Ff5e8cd08c58a721A38Aaf62779478].

```

## Fixed Issue(s)
No issue raised for this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-19 10:23:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6436" class=".btn">#6436</a>
            </td>
            <td>
                <b>
                    Implement "pending" for qbft_getValidatorsByBlockNumber
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
This PR adds support for "pending" as a string in qbft_getValidatorsByBlockNumber.

It returns the validators for the block that is in the process of being mined.

In certain stalled-chain scenarios where a new validator has been voted in but not enough validators are online to mine the next block, neither `qbft_getPendingVotes` nor `qbft_getValidatorsByBlockNumber("latest")` are useful since the vote is no longer pending, and the "latest" block is not the one that is failing to be mined. Similarly, `qbft_getValidatorsByBlockNumber(<next-block-number>)` cannot be used because the next block doesn't exist yet.

"pending" already exists as a block string, but isn't implemented by most JSON/RPC methods. This is only the 2nd method that implements it I believe, but it seems like a valid interpretation of "pending" in this case. All other JSON/RPC methods will continue to revert to "latest" if "pending" is specified.

## Fixed Issue(s)
No issue raised for this.

## Doc changes required

- I think https://besu.hyperledger.org/public-networks/how-to/use-besu-api/json-rpc#block-parameter needs updating to say "Use only with [eth_getTransactionCount](https://besu.hyperledger.org/public-networks/reference/api#eth_gettransactioncount) and [qbft_getValidatorsByBlockNumber](https://besu.hyperledger.org/private-networks/reference/api#qbft_getvalidatorsbyblocknumber)"
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-19 10:07:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6435" class=".btn">#6435</a>
            </td>
            <td>
                <b>
                    24.1.1-RC
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
        Created At 2024-01-19 08:34:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6432" class=".btn">#6432</a>
            </td>
            <td>
                <b>
                    prep for release 24.1.1
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
        Created At 2024-01-19 06:27:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6431" class=".btn">#6431</a>
            </td>
            <td>
                <b>
                    EOF Spec Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update a few EOF features based on updated spec
* Add a prague reference test target
* Run evmtool from prestate when no code specified
* RETF and dangling immediate arg fixes

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
        Created At 2024-01-19 05:51:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6427" class=".btn">#6427</a>
            </td>
            <td>
                <b>
                    GitHub Actions CI/CD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Proposed alternative to using CircleCI.

Please also consider the Design Doc available here: https://wiki.hyperledger.org/pages/viewpage.action?pageId=80774216

Fixes #6238 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-18 19:40:58 +0000 UTC
    </div>
</div>

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
                    Upgrade Prometheus and Opentelemetry dependencies
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

Upgrade Prometheus and Opentelemetry dependencies, and adjust the code accordingly.

Prometheus simpleclient upgrade introduces some changed, to follow the OpenMetrics specification, like adding the `_total` suffix to every counters that haven't it, and adding a `_created` suffixed metric to some types, while the latter is not an issue, the `_total` suffix is a breaking change, and requires an updated version of our official Grafana dashboard, that has been already [published here](https://grafana.com/grafana/dashboards/16455-besu-full/), and is compatible with both metrics names.
Using the metrics by other means require a change to the tooling, for this a breaking change section has been added.

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

