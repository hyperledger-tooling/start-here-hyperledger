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

