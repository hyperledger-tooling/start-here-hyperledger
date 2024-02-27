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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6599" class=".btn">#6599</a>
            </td>
            <td>
                <b>
                    Ensure halt reasons in TraceFrames in `DebugOperationTracer.tracePostExecution`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This PR fixes the debug trace series generation for `opcodes` that do not set an explicit `ExceptionalHaltReason` in the `OperationResult`. Previously, operations like `dup5` could lead to an exceptional halt (e.g., due to running out of gas) without this being accurately captured in the trace output, as the halt reason was not set explicitly. This situation affected the `FlatTraceGenerator's` ability to accurately reflect halt conditions and `subtrace` counts.

The `DebugOperationTracer.tracePostExecution` method has been updated to check the `MessageFrame` for an exceptional halt reason if it's absent in the `OperationResult`. This adjustment aligns with the existing approach used by the `StandardJsonTracer`

The trace output for the transaction referenced in the [issue](https://github.com/hyperledger/besu/issues/6591) now accurately displays the correct halt reason and appropriately counts subtraces.

```diff
{
   "jsonrpc":"2.0",
   "id":1,
   "result":[
      {
         "action":{
            "callType":"call",
            "from":"0xd8422593f16cd6d65c3f4cfa28b5b5a862037123",
            "gas":"0x1a18",
            "input":"0x5b7d7482000000000000000000000000000000000000000000000000000000000000004000000000000000000000000000000000000000000000000000000000000000a0000000000000000000000000000000000000000000000000000000000000004034313465376364326235656636313337656166383661396134653064666430333536313063323562323536333031633662396361356361313531653233373965000000000000000000000000000000000000000000000000000000000000004034646163313738646333376331303736346235643862373862633135323635366437316662343865626537396361613835343437336530663031313132313732",
            "to":"0xd1a3abf42f9e66be86cfdea8c5c2c74f041c5e14",
            "value":"0x0"
         },
         "blockHash":"0x2345afc92f072449294eba81a33116da5d014e74ecbe5db53e5d72b40145976f",
         "blockNumber":2160351,
-        "result": {
-           "gasUsed": "0x0",
-           "output": "0x"
-        },
-        "subtraces": 0,
+       "error":"Out of gas",
+       "subtraces":1,
        "traceAddress":[
            
         ],
         "transactionHash":"0xea89b8082ab1e9e8f0a025ead197ce8e2cdf4b1212d4ec13a91e97570485a053",
         "transactionPosition":0,
         "type":"call"
      },
      {
         "action":{
            "callType":"delegatecall",
            "from":"0xd1a3abf42f9e66be86cfdea8c5c2c74f041c5e14",
            "gas":"0x6dd",
            "input":"0x5b7d7482000000000000000000000000000000000000000000000000000000000000004000000000000000000000000000000000000000000000000000000000000000a0000000000000000000000000000000000000000000000000000000000000004034313465376364326235656636313337656166383661396134653064666430333536313063323562323536333031633662396361356361313531653233373965000000000000000000000000000000000000000000000000000000000000004034646163313738646333376331303736346235643862373862633135323635366437316662343865626537396361613835343437336530663031313132313732",
            "to":"0x564477025731ee7197eecf2c4a0d0106cc3e4572",
            "value":"0x0"
         },
         "blockHash":"0x2345afc92f072449294eba81a33116da5d014e74ecbe5db53e5d72b40145976f",
         "blockNumber":2160351,
-        "result": {
-           "gasUsed": "0xffffffffffffece0",
-            "output": "0x"
-         },
+       "error":"Out of gas",
         "subtraces":0,
         "traceAddress":[
            0
         ],
         "transactionHash":"0xea89b8082ab1e9e8f0a025ead197ce8e2cdf4b1212d4ec13a91e97570485a053",
         "transactionPosition":0,
         "type":"call"
      }
   ]
}

```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 04:41:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6598" class=".btn">#6598</a>
            </td>
            <td>
                <b>
                    PR Template updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - replaces comment on PR with template like the one used for opening an issue.
- makes test workflows manually runnable via workflow_dispatch
- updates to latest version of gradle build action
- corrects login to ghcr on nightly builds
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 02:33:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6596" class=".btn">#6596</a>
            </td>
            <td>
                <b>
                    Clique block period transition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span><span class="chip">TeamGroot</span>
            </td>
            <td>
                Add [BFT-style transitions](https://besu.hyperledger.org/private-networks/how-to/configure/consensus/qbft#transitions) to Clique, modelled with `ForksSchedule<CliqueConfigOptions>`

CliqueMiningAcceptanceTest heavily inspired by [BftBlockRewardPaymentAcceptanceTest](https://github.com/hyperledger/besu/blob/main/acceptance-tests/tests/src/test/java/org/hyperledger/besu/tests/acceptance/bft/BftBlockRewardPaymentAcceptanceTest.java)

Preparatory story to https://github.com/hyperledger/besu/issues/6290 - a `createemptyblocks` transition will be added in the next PR.

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
          "blockperiodseconds": 1
        },
        {
          "block": 6,
          "blockperiodseconds": 2
        },
      ]
    }
  },
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 07:34:52 +0000 UTC
    </div>
</div>

