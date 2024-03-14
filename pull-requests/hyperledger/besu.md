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
                PR <a href="https://github.com/hyperledger/besu/pull/6734" class=".btn">#6734</a>
            </td>
            <td>
                <b>
                    Change eth trace from 'Message not expected' to 'Request message'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Change the trace entry for messages that aren't `response`-type messages.

## Fixed Issue(s)
N/A
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 14:27:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6733" class=".btn">#6733</a>
            </td>
            <td>
                <b>
                    Add comments to a couple of the the EthPeer methods to clarify their behaviour
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Very minor PR to add some javadoc comments to 2 methods

## Fixed Issue(s)
N/A
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 14:06:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6731" class=".btn">#6731</a>
            </td>
            <td>
                <b>
                    allow empty maxFeePerBlobGas for eth_call
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
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [x] locally run all unit tests via: `./gradlew build`
- [x] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [x] locally run all integration tests via: `./gradlew integrationTest`
- [x] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

## Fixed Issue(s)
fixes #6709
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 08:39:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6730" class=".btn">#6730</a>
            </td>
            <td>
                <b>
                    chore: remove repetitive words
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 06:20:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6729" class=".btn">#6729</a>
            </td>
            <td>
                <b>
                    Change ProcessBesuNodeRunner and ThreadBesuNodeRunner to use DEFAULT_BONSAI_CONFIG
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [x] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

## Fixed Issue(s)
Fixes #6583
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 05:42:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6728" class=".btn">#6728</a>
            </td>
            <td>
                <b>
                    [MINOR] Move potentially spammy peer discovery warn log to debug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For one user, this log was appearing every couple of seconds.

We determined that it shouldn't affect the peers required for the node to function therefore there's potentially nothing to act on WARN level is too high.

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
        Created At 2024-03-14 05:20:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6727" class=".btn">#6727</a>
            </td>
            <td>
                <b>
                    Refactor AbstractGasLimitSpecification to simplify isValidTargetGasLimit bound condition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Refactor AbstractGasLimitSpecification to simplify isValidTargetGasLimit bound condition. This was reported during errorprone plugin update.

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
        Created At 2024-03-13 23:49:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6726" class=".btn">#6726</a>
            </td>
            <td>
                <b>
                    Refactor StorageRangeDataRequest to fix unused variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Refactor StorageRangeDataRequest to fix unused variable. Reporting during update of errorprone plugin.

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
        Created At 2024-03-13 23:36:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6725" class=".btn">#6725</a>
            </td>
            <td>
                <b>
                    Refactor PluginPrivacyController to fix parameter name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Refactor PluginPrivacyController. Fix parameter name to match overridden method. Identified during errorprone plugin update.

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
        Created At 2024-03-13 23:24:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6723" class=".btn">#6723</a>
            </td>
            <td>
                <b>
                    pull_req instead of target
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Removes annotation of failed tests onto pr, since we have to run them before review anyway. 

### Thanks for sending a pull request! Have you done the following?

- [X] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [X] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [X] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [X] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-13 17:58:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6721" class=".btn">#6721</a>
            </td>
            <td>
                <b>
                    diffbased refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Here's a breakdown of the PR:

- Splitting Bonsai: The PR aims to divide Bonsai into two packages

- Common Classes with a Prefix: The common part will include classes prefixed with "DiffBased." These classes are designed to provide a base for both Bonsai and any future storage format that might use this diff-based approach.

- Bonsai's Specifics: Bonsai will retain its unique features in its own package. This means that while it shares the diff-based infrastructure with the common part, it also has its own specific functionalities that are not shared with other storage format.

- Extension to Verkle: this modification add the possibility of adding "Verkle" as a new storage format based on the diff-based architecture. Like Bonsai, Verkle would use the common diff-based classes but also have its own specific features.

In summary, the pull request proposes restructuring Bonsai to make it more modular and efficient. This not only improves data management within Bonsai but also sets the stage for incorporating new format like Verkle, which can share the common base while having their unique functionalities.


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
        Created At 2024-03-13 11:04:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6720" class=".btn">#6720</a>
            </td>
            <td>
                <b>
                    add check for sync status to fix flaky tests
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
- [x] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

## Fixed Issue(s)
Hopefully this fixes #6719 and #6718
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-13 03:02:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6716" class=".btn">#6716</a>
            </td>
            <td>
                <b>
                    Refactor BadBlockReason enum out of BadBlockCause
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
BadBlockReason was an non-static inner enum in BadBlockCause and it was used in static context. This caused one of our custom errorprone checks to not pick up the "method param not final argument" correctly. Refactoring it out as an static top level class. Now all the checks are applied correctly.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#6685 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-12 23:18:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6713" class=".btn">#6713</a>
            </td>
            <td>
                <b>
                    [MINOR] Remove unused method
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
        Created At 2024-03-12 00:36:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6712" class=".btn">#6712</a>
            </td>
            <td>
                <b>
                    edits to changelog for 24.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * correct release number for 24.3.0
* added link to release page (not individual download links)
* correction to X_SNAP X_CHECKPOINT removal target version
* move blob RPC changes into 24.3.0
* BFT (not PoA) won't start with SNAP or CHECKPOINT

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
        Created At 2024-03-12 00:23:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6711" class=".btn">#6711</a>
            </td>
            <td>
                <b>
                    [minor] Add privacy and permissioning services to thread plugin context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add privacy and permissioning services to thread plugin context

## Fixed Issue(s)
fixes #6691 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-12 00:18:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6708" class=".btn">#6708</a>
            </td>
            <td>
                <b>
                    Change`txpool_beusPendingTransactions`:`numResults`  from a required parameter to an optional parameter 
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
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description
Enhancement `TX_POOL` API `txpool_besuPendingTransactions` by changing 'numResults' from a required parameter to an optional parameter.  if the parameter `limit` does not exist will use pending transactions size as a limit.

## Fixed Issue(s)
fixes #6707 
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-11 09:25:07 +0000 UTC
    </div>
</div>

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
                <span class="chip">doc-change-required</span>
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

fixes #6714

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

