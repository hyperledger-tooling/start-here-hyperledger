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

