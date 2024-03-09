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
                PR <a href="https://github.com/hyperledger/besu/pull/6705" class=".btn">#6705</a>
            </td>
            <td>
                <b>
                    Gha updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

## Fixed Issue(s)

fixes #6695 

- No longer defers testing till after approval, functionality to be redesigned
- concurrent runs for the same branch will be cancelled on update to the ref
- new develop floating pre-release to be maintained with downloadable artifacts on push to main
- codeql job deferred to nightly runs on main

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [x] locally run all unit tests via: `./gradlew build`
- [x] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [x] locally run all integration tests via: `./gradlew integrationTest`
- [x] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-08 19:10:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6702" class=".btn">#6702</a>
            </td>
            <td>
                <b>
                    Transaction call object to accept both input and data field if equal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [X] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [X] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [X] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description
https://github.com/hyperledger/besu/pull/6094 introduced the option to provide the calldata via the input field instead of the deprecated data field. It also introduced a check that prevents both field from being set. This seems overly strict as it prevents clients from setting both fields to remain backward-compatible. This PR relaxes the check to only fail if both fields are set and they are not equal.

## Fixed Issue(s)
fixes #6697 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-08 15:07:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6701" class=".btn">#6701</a>
            </td>
            <td>
                <b>
                    Draft - Do not merge - Multi version flat db rebase
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-08 04:03:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6700" class=".btn">#6700</a>
            </td>
            <td>
                <b>
                    Enhanced control over plugins registration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">plugins</span>
            </td>
            <td>
                ## PR description
This PR introduces improvements to the plugin registration logic in Besu, providing users with granular control over the registration of plugins. Previously, Besu attempted to register all plugins found in the plugins directory indiscriminately. With this update, users can now specify exactly which plugins should be registered, halting the application startup if any specified plugin does not exist. This feature is beneficial for environments where precise plugin configurations are necessary.

### CLI Options and Configuration Profiles
The new plugin registration logic introduces one CLI options:

`--plugins`: Specifies a comma-separated list of plugin names to be registered.

### Changes

- Plugins Registration Logic: Users can now specify a list of plugins to be registered via CLI options. This list determines which plugins Besu will attempt to register. Besu validates the presence of each specified plugin in the plugins directory. If any specified plugin is not found, the application will halt, preventing startup with an incomplete set of plugins. Any plugin found in the directory that is not explicitly required will be ignored.

### Examples

`besu  --plugins=essential-plugin,security-plugin`

In this scenario, if either "essential-plugin" or "security-plugin" is not found in the specified directory, Besu will halt, signalling a configuration issue that needs resolution. Any other plugins will be ignored.

It can also be defined in TOML configuration profiles.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-08 02:45:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6699" class=".btn">#6699</a>
            </td>
            <td>
                <b>
                    proposed "develop" build versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
As part of our recent build and release changes, we no longer need to explicitly maintain the build version in gradle.properties file.

This PR is a proposal to change our "develop" builds to use git commit and HEAD details to specify a dynamic build version.

for example this PR, prior to committing the changes, produced a build named:
`besu-24.3.7-develop-610927511e.tar.gz`

After committing the gradle changes and rebuilding, it produced a build named:
`besu-24.3.7-develop-600d812d89.tar.gz`


Open to suggestions, feedback, and identifying corner cases




## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 23:30:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6698" class=".btn">#6698</a>
            </td>
            <td>
                <b>
                    Support pruned chain history in peer validators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Change the behavior of peer block validator to allow block absence to be tolerated for some rules, specifically DaoForkPeerValidator, in support of:
* https://eips.ethereum.org/EIPS/eip-4444
* https://github.com/ethereum/EIPs/pull/8266
* and besu checkpoint sync'd nodes


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 21:34:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6696" class=".btn">#6696</a>
            </td>
            <td>
                <b>
                    fix for txpool inSync listener to honor initial sync state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix and unit test for transaction pool inSync listener to ensure we account for initial sync state when enabling/disabling the pool.

The inSync listener responds to chain events only and does not take into account worldstate sync.  This pr adds an additional initial sync condition in the sync listener to ensure we do not enable the pool when the chain sync finishes, but the worldstate is incomplete (like in the case of a debug_resyncWorldState)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 19:57:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6693" class=".btn">#6693</a>
            </td>
            <td>
                <b>
                    Add logging for newer FCU payload parameter details
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Simon Dudley <simon.dudley@consensys.net>

### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 07:43:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6692" class=".btn">#6692</a>
            </td>
            <td>
                <b>
                    Use external custom error prone dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description
Use external custom error prone dependency. 
TODO: Use Hyperledger published dependency
TODO: Custom errorprone checks are applied.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 06:07:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6688" class=".btn">#6688</a>
            </td>
            <td>
                <b>
                    [build] - Update gradle build to invoke int test compile task on assemble task
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [x] locally run all unit tests via: `./gradlew build`
- [x] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [x] locally run all integration tests via: `./gradlew integrationTest`
- [x] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description
The `assemble` task has been modified to additionally depends on `compileIntegrationTestJava` so that any compilation issues are reported earlier locally and in CI.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #6670 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 03:09:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6687" class=".btn">#6687</a>
            </td>
            <td>
                <b>
                    eth_call with blobs - added more spec tests 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
* Added some more tests for specific error conditions
* corrected a validation message

## Fixed Issue(s)
refs #6657

### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [x] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 02:04:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6686" class=".btn">#6686</a>
            </td>
            <td>
                <b>
                    Transaction simulation service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

Introduce `TransactionSimulationService` so plugins can simulate txs processing

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-06 18:43:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6684" class=".btn">#6684</a>
            </td>
            <td>
                <b>
                    Silence vertx dns errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description
quickie pr to silence the vertx counterpart to the tuweni dns errors

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 20:06:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6683" class=".btn">#6683</a>
            </td>
            <td>
                <b>
                    [fix] Minor documentation fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [x] locally run all unit tests via: `./gradlew build`
- [x] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [x] locally run all integration tests via: `./gradlew integrationTest`
- [x] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 14:44:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6682" class=".btn">#6682</a>
            </td>
            <td>
                <b>
                    test rc2 with snap fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 08:26:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6681" class=".btn">#6681</a>
            </td>
            <td>
                <b>
                    RC4 - eth_call and eth_feeHistory add blob fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-picks #6679 and #6661 for blob support

### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 06:11:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6679" class=".btn">#6679</a>
            </td>
            <td>
                <b>
                    Add blobs to `eth_feeHistory`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add blob fields to eth_fee_History

## Fixed Issue(s)
fixes #6580

On Sepolia:
`curl -H "Content-Type: application/json" -d '{"id": 1, "jsonrpc": "2.0", "method": "eth_feeHistory", "params": ["0x5", "0x526006", [20,30]] }' http://127.0.0.1:8545/ | jq .
`
```
{
  "jsonrpc": "2.0",
  "id": 1,
  "result": {
    "oldestBlock": "0x526002",
    "baseFeePerGas": [
      "0x4506f",
      "0x43d32",
      "0x44d30",
      "0x42021",
      "0x39c1d",
      "0x38cd0"
    ],
    "baseFeePerBlobGas": [
      "0x4a1bd3218",
      "0x502994693",
      "0x4d137e31b",
      "0x4741676a3",
      "0x3f5694c1f",
      "0x4741676a3"
    ],
    "gasUsedRatio": [
      0.4303144,
      0.5589600333333333,
      0.3363257666666667,
      0,
      0.4337706333333333
    ],
    "blobGasUsedRatio": [
      0.8333333333333334,
      0.3333333333333333,
      0.16666666666666666,
      0,
      1
    ],
    "reward": [
      [
        "0x186a1",
        "0x186a1"
      ],
      [
        "0x186a1",
        "0x186a1"
      ],
      [
        "0x59682f00",
        "0x59682f00"
      ],
      [
        "0x0",
        "0x0"
      ],
      [
        "0x3b9aca00",
        "0x3b9aca00"
      ]
    ]
  }
}
```


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 00:26:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6678" class=".btn">#6678</a>
            </td>
            <td>
                <b>
                    Bugfix - only track intrinsically bad blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This is a follow-up to PR https://github.com/hyperledger/besu/pull/6622.  Rework bad block handling so that we are only tracking blocks that are intrinsically bad due to a spec-related validation error.  We should not be marking blocks as bad if we are missing data locally or encounter some unspecified exception during block processing.  

## Fixed Issue(s)
Tangentially related to https://github.com/hyperledger/besu/issues/6301

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 22:07:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6677" class=".btn">#6677</a>
            </td>
            <td>
                <b>
                    Revert "Acceptance tests to use bonsai (#6619)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 647750c201dcd06fac51028bfb93e6242c2e222b.

### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 17:45:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6676" class=".btn">#6676</a>
            </td>
            <td>
                <b>
                    Make block txs selection max time aware of PoA transitions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

As a follow up of #6596 this PR makes the block txs selection max time, correctly  aware of the PoA transitions, while before only the block period from the genesis was used, while that value can change according to the transitions defined in the genesis file. To support that the `genesisBlockPeriodSeconds` has been renamed to `blockPeriodSeconds` and the configuration is now modifiable at runtime, according to the transitions schedule.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 16:20:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6675" class=".btn">#6675</a>
            </td>
            <td>
                <b>
                    Don't start the BFT mining coordinator when it is created, just enable it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
When creating a BFT mining coordinator, if the sync phase is already complete then enable the coordinator but don't start it.

Start will be done either during starting of the ethereum main loop, or on receiving an event notification that syncing has completed.

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/6674
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 13:47:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6672" class=".btn">#6672</a>
            </td>
            <td>
                <b>
                    clean-up: Remove isChainPruneEnabled from MergeContext interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [x] locally run all unit tests via: `./gradlew build`
- [x] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [x] locally run all integration tests via: `./gradlew integrationTest`
- [x] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description
This PR removes some tech debit that was introduce due with the chain pruner. This is not used or necessary anymore after PR https://github.com/hyperledger/besu/pull/4703

Tested:
- [x] Sepolia with chain pruning disable
- [x] Sepolia with chain pruning enabled
- [x] Mainnet with chain pruning disable
- [x] Mainnet with chain pruning enabled
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 05:32:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6667" class=".btn">#6667</a>
            </td>
            <td>
                <b>
                    allow snap/checkpoint with clique
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Docs - can't see anywhere in the docs where we mention snap or checkpoint on the private networks side, but may be worth adding an explicit note that you must use FAST or FULL if using BFT consensus.

### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

## Fixed Issue(s)
Adjustment to #6625
Fixes https://github.com/hyperledger/besu/issues/6385
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-03 21:53:00 +0000 UTC
    </div>
</div>

