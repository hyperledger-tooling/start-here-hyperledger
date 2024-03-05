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
                <span class="chip">doc-change-required</span>
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
                    Make block txs selection max time aware of PoA transactions
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

As a follow up of #6596 this PR makes the block txs selection max time, correctly  aware of the PoA transactions, while before only the block period from the genesis was used, while that value can change according to the transitions defined in the genesis file. To support that the `genesisBlockPeriodSeconds` has been renamed to `blockPeriodSeconds` and the configuration is now modifiable at runtime, according to the transitions schedule.

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
                <span class="chip">doc-change-required</span>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6666" class=".btn">#6666</a>
            </td>
            <td>
                <b>
                    Update Vert.x to 4.5.4
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
        Created At 2024-03-01 19:35:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6665" class=".btn">#6665</a>
            </td>
            <td>
                <b>
                    Fix txpool dump/restore race condition
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

The disk access was not properly guarded against overlapping dump/restore tasks

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #6664 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 16:46:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6661" class=".btn">#6661</a>
            </td>
            <td>
                <b>
                    Eth call with 4844 params
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Added support for `maxFeePerBlobGas` and `versionedHashes` to eth_call 

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
refs #6657 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 07:28:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6659" class=".btn">#6659</a>
            </td>
            <td>
                <b>
                    [MINOR] Remove todo override genesis config
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

## Fixed Issue(s)
builds on #6654 
see #3874 - removed TODOs from BesuCommandTest
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 03:13:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6654" class=".btn">#6654</a>
            </td>
            <td>
                <b>
                    [MINOR] adjust help message for --genesis-file
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

## Fixed Issue(s)
fixes #5877
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 01:38:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6648" class=".btn">#6648</a>
            </td>
            <td>
                <b>
                    Update commons-compress to 1.26.0
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
        Created At 2024-02-29 17:56:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6647" class=".btn">#6647</a>
            </td>
            <td>
                <b>
                    fix snap candidate
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
        Created At 2024-02-29 17:53:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6646" class=".btn">#6646</a>
            </td>
            <td>
                <b>
                    Retrieve all transaction receipts for a block in one request
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
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [ ] locally run all unit tests via: `./gradlew build`
- [ ] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [ ] locally run all integration tests via: `./gradlew integrationTest`
- [ ] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

1. Retrieve all transaction receipts in a block in 1 call to blockchain query instead of a call for each transaction in a block
2. Calculate transaction fee reward for miner based on `effectivePriorityFeePerGas` instead of `effectiveGasPrice` because `baseFee` would be burnt.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 13:54:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6644" class=".btn">#6644</a>
            </td>
            <td>
                <b>
                    Besu command test split
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refs #6428 
* split out some tests into separate test classes
* Also use tempDir for the `dataDirOptionMustBeUsed` test to avoid leaving behind `besu/VERSION_METADATA.json` file

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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 07:11:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6643" class=".btn">#6643</a>
            </td>
            <td>
                <b>
                    revert 6499 flat-db-healing-enabled false by default
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 00:19:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6642" class=".btn">#6642</a>
            </td>
            <td>
                <b>
                    revert 6499 flat-db-healing-enabled false by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverted since there's an issue with snap sync that is revealed by not being able to turn off this flag.

refs https://github.com/hyperledger/besu/issues/6157

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
        Created At 2024-02-29 00:08:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6641" class=".btn">#6641</a>
            </td>
            <td>
                <b>
                    Feature/fleet mode rebase
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
rebase onto main of the services refactor for fleet mode, see original #6003

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-28 21:20:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6640" class=".btn">#6640</a>
            </td>
            <td>
                <b>
                    Snap server rebase
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
        Created At 2024-02-28 21:14:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6636" class=".btn">#6636</a>
            </td>
            <td>
                <b>
                    Refactor and extend PluginTransactionPoolValidatorService
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

This PR extends the transaction pool validator plugin, to also pass the `isLocal` and `hasPriority` attributes of the tx to validate
```
Optional<String> validateTransaction(
      final Transaction transaction, final boolean isLocal, final boolean hasPriority);
```
Then a renaming has been done, for making clear that this validator service only apply when adding a tx to the transaction pool, and not when doing other validations, like during block import, along with a refactor to align this service to the way TransactionSelectorService is managed.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-28 16:47:01 +0000 UTC
    </div>
</div>

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
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Fixes #6385 

Docs - can't see anywhere in the docs where we mention snap or checkpoint on the private networks side, but may be worth adding an explicit note that you must use FAST or FULL if using BFT consensus.


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [x] locally run all unit tests via: `./gradlew build`
- [x] locally run all acceptance tests via: `./gradlew acceptanceTest`
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

Summary of changes:
- Require a `BadBlockCause` when pushing blocks to `BadBlockManager`
- Simplify bad block checks by adding utility method `BadBlockManager.isBadBlock`
- Add some basic tests for `BadBlockManager`
- In event handler `MergeCoordinator.onBadChain`, only push descendants of the bad block to the`BadBlockManager`.  The bad block itself will already have been pushed into the `BadBlockManager` when processed in `MainnetBlockValidator` and the `MergeCoordinator` does not have the context on why the bad block was marked as bad.
- Remove unused API `MergeMiningCoordinator.addBadBlock`
- Fix / add tests to `MainnetBlockValidatorTest` 
   - Add tests for `fastBlockValidation()`
   - Set all mocks upfront to ensure every test executes from a baseline of success. Previously several tests were passing artificially.  The mocks were not set up correctly so some tests were not hitting the cases that were intended. 
- Create some factory methods on `InvalidBlockException` to handle cases where (previously required) block data is not available
- Disambiguate a few different types of errors in `DownloadHeaderSequenceTask` and add tests

## Fixed Issue(s)
Part of #6301
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 23:51:35 +0000 UTC
    </div>
</div>

