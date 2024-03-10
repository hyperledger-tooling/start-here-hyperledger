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

