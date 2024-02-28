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
                PR <a href="https://github.com/hyperledger/besu/pull/6625" class=".btn">#6625</a>
            </td>
            <td>
                <b>
                    prevent startup if PoA and snap/checkpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #6385 

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

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
        Created At 2024-02-28 05:58:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6624" class=".btn">#6624</a>
            </td>
            <td>
                <b>
                    feat: add fixed basefee options
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
Add `fixedBaseFee` options to forced `baseFee` same as `gasPrice` value.


I'm new to the Java language, please guide any aspects I can further improve or modify.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
https://github.com/hyperledger/besu/issues/6335

## Revised PR
https://github.com/hyperledger/besu/pull/6562
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-28 05:14:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6622" class=".btn">#6622</a>
            </td>
            <td>
                <b>
                    [#6301] Track bad block cause
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Track bad block causes in `BadBlockManager` in preparation for exposing plugin events.  This data is useful because a consumer may want to take a different action depending on the cause.  For example, for #6301, we probably want to trace blocks with an actual validation error and ignore blocks that just descend from a bad block. 

## Fixed Issue(s)
Part of #6301
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 23:51:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6619" class=".btn">#6619</a>
            </td>
            <td>
                <b>
                    Acceptance tests to use bonsai
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #6583 

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
        Created At 2024-02-27 11:03:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6618" class=".btn">#6618</a>
            </td>
            <td>
                <b>
                    Cleanup after refactoring `TransactionSelectionService`
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

Just some more code that can be removed

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 10:21:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6616" class=".btn">#6616</a>
            </td>
            <td>
                <b>
                    Fix NPE when running revert variable subcommand
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
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description
Fixes NPE when running the revert variables subcommand. 

Due to changes in how the data storage configuration is handled the approach of using the storage provider directly from the `BesuSubcommand` no longer works. Instead changed the approach that to use what was used in the trielog subcommands and creates the BesuController using the `BesuCommand.buildController()` to get access to the `StorageProvider`. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #6614
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 03:38:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6611" class=".btn">#6611</a>
            </td>
            <td>
                <b>
                    Make layered txpool aware of minGasPrice and minPriorityFeePerGas dynamic options
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

This PR improved the quality of the txs that are kept in the prioritized layer of the layered txpool, taking in account also the dynamic value of the `minGasPrice` and `minPriorityFeePerGas` options.
So if a tx effective gas price is below the current value of `minGasPrice` or its effective priority fee is below the `minPriorityFeePerGas` it is not kept, or promoted, in the prioritized layer, since it will not be selected during block creation.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-26 13:57:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6609" class=".btn">#6609</a>
            </td>
            <td>
                <b>
                    Check for snap server
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
When we are connecting to an EthPeer and we are doing snap sync find out whether that peer does serve snap data.
This is needed to make sure that we have a minimum of snap data serving peers and to make sure that we only send snap requests to peers that serve snap data.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-23 04:31:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6608" class=".btn">#6608</a>
            </td>
            <td>
                <b>
                    Clique createemptyblocks transition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
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

Create genesis config transitions:
```
  "config": {
    ...
    "clique": {
      "blockperiodseconds": 3,
      "epochlength": 30,
      "requesttimeoutseconds": 6,
      "createemptyblocks": true
    },
    "transitions": {
      "clique": [
        {
          "block": 3,
          "createemptyblocks": false
        }
      ]
    }
  },
```

Built on top of https://github.com/hyperledger/besu/pull/6596

Diff for easier review before #6596 is merged: https://github.com/siladu/besu/compare/clique_transition_blocks...clique-transition-createemptyblocks


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #6290 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-23 03:44:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6606" class=".btn">#6606</a>
            </td>
            <td>
                <b>
                    Abstracts out which container registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Abstracts out which container registry to point to, anticipating an eventual transition from docker.io to ghcr.io
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-22 15:39:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6605" class=".btn">#6605</a>
            </td>
            <td>
                <b>
                    During version check, create data dir if it doesn't exist
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Resolves breaking change in PR https://github.com/hyperledger/besu/pull/6307 that blocks Besu startup if the data dir doesn't exist already
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-22 08:23:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6604" class=".btn">#6604</a>
            </td>
            <td>
                <b>
                    [MINOR] Rotate changelog since 24.2.0-RC has been cut
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
        Created At 2024-02-22 06:04:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6603" class=".btn">#6603</a>
            </td>
            <td>
                <b>
                    Remove unnecessary PoS checkpoint methods and variables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [x] locally run all unit tests via: `./gradlew build`
- [x] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [x] locally run all integration tests via: `./gradlew integrationTest`
- [x] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description
This PR removes unnecessary checks and variables used to work around the latestValidAncestorDescendsFromTerminal from PoW, which has been removed by PR https://github.com/hyperledger/besu/pull/4703
- Test done:
- [x] Synced Sepolia successfully
- [x] Synced Goerli successfully
- [x] Synced Mainnet successfully

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-22 04:42:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6602" class=".btn">#6602</a>
            </td>
            <td>
                <b>
                    Reduce receipt size
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
Reduce receipt by introducing a new compact receipt encoding

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-22 02:55:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6600" class=".btn">#6600</a>
            </td>
            <td>
                <b>
                    Gha docker pull
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

Now appends the correct docker pull command to the release notes, i.e.

`docker pull ghcr.io/hyperledger/besu:24.2.0-RC1`

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 16:17:52 +0000 UTC
    </div>
</div>

