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
                PR <a href="https://github.com/hyperledger/besu/pull/6880" class=".btn">#6880</a>
            </td>
            <td>
                <b>
                    Log detailed timing of block creation steps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

if log level is at debug, detailed timing of block creation steps are logged, along with the standard block info.

Log will look like this:

```
2024-04-05 10:54:46.962+00:00 | MinerExecutor | INFO  | BlockMiner | Produced #260,775 / 63 tx / 0 om / 1,577,124 (2.6%) gas / (0xb6907722d13c36fb54747d11f4b7c734d6b57035ca1a3428e4b5c9f347644b63) in 0.000s, timing [Started at 2024-04-05T10:54:46.693633274Z, protocolWait=254ms, duplicateWorldState=0ms, preTxsSelection=3ms, txsSelection=9ms, blockAssembled=1ms, importingBlock=0ms, notifyListeners=0ms, log=0ms]
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-04 15:35:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6879" class=".btn">#6879</a>
            </td>
            <td>
                <b>
                    fix: Use HttpRequest authority instead of host
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
fix: Use HttpRequest authority instead of host.
- Use authority method to determine the host name from header instead of using deprecated host method
- Fix WebSocketService unit test

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #6878 

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [x] acceptance tests: `./gradlew acceptanceTest`
- [x] integration tests: `./gradlew integrationTest`
- [x] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-04 00:18:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6877" class=".btn">#6877</a>
            </td>
            <td>
                <b>
                    Relax PeerReputation timeout threshold
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Relax the peer timeout threshold, align with EthPeer max outstanding requests


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 17:15:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6876" class=".btn">#6876</a>
            </td>
            <td>
                <b>
                    Snap protocol always enabled
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes bug where disabling snap server disables snap protocol

### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 15:05:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6875" class=".btn">#6875</a>
            </td>
            <td>
                <b>
                    Add debug logs for when transaction processing halts or reverts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR adds `debug` level logs to the transaction processor in the event of either:

1. transaction processing halting (e.g. a post-shanghai transaction submitted to a pre-shanghai fork node)
2. the transaction reverting

Currently in order to see the reason for a transaction revert you typically have to either:

- Have `--revert-reason-enabled` on the node, and capture the revert reason in the application or trace the receipt response 
- Have the `DEBUG` JSON/RPC API enabled and use the `debug_traceTransaction` JSON/RPC call

In some scenarios it is useful not to have to enable revert reasons and or use JSON/RPC calls to see the revert reasons. Instead simply turning `DEBUG` logging on for the `MainnetTransactionProcessor` will now let you see the reason for a revert (or a halt).

I considered making it a `TRACE` log instead of `DEBUG` log but my view is that the output is fairly short (not lines and lines of output), transactions are unlikely to revert that frequently, and `TRACE` adds a fair amount of extra noise to the output. Happy to take others comments on whether it should be `TRACE` though.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 13:40:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6874" class=".btn">#6874</a>
            </td>
            <td>
                <b>
                    Blob transaction replacement rule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description

Add `tx-pool-blob-price-bump` option to configure the price bump percentage required to replace blob transactions (by default 100%), also a blob tx can only replace and be replaced by another blob tx.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 10:12:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6873" class=".btn">#6873</a>
            </td>
            <td>
                <b>
                    Move log entry to specific places where it is useful
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Reduce BFT validator log noise

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/6872


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 08:41:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6871" class=".btn">#6871</a>
            </td>
            <td>
                <b>
                    Fix besu-untuned start script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 08:01:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6870" class=".btn">#6870</a>
            </td>
            <td>
                <b>
                    [MINOR] nuke those extra ellipses
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span><span class="chip">peering</span>
            </td>
            <td>
                ## PR description

Similar to #6849 - ellipsis is now included in loggableId. There were a few more places where this was duplicated.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 06:43:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6867" class=".btn">#6867</a>
            </td>
            <td>
                <b>
                    Add prefix to dns on holesky
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR adds the missing enrtree prefix to the dns address of the holesky network. Kudos to @matkt for picking up this one.


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 01:15:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6866" class=".btn">#6866</a>
            </td>
            <td>
                <b>
                    use event name instead of ref, which may be non-deterministic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

An interesting subtlety of the github api is that when referring to a ref, there may be multiple and they are sorted alphabetically. So if we assume that the version to use in the build is what we tagged it as, we will only get the right value if the second tag is alphabetically earlier.

This fixes it by using whatever name is given to the release. Don't be clever, just use calver for now!

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 21:28:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6865" class=".btn">#6865</a>
            </td>
            <td>
                <b>
                    One JDK to rule them all
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Reduces the number of JDKs used in various docker images to only OpenJDK 21
Simplifies gradle build scripts to accomodate

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #6703 
fixes #6722 


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 17:58:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6861" class=".btn">#6861</a>
            </td>
            <td>
                <b>
                    Remove some dead code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 12:59:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6860" class=".btn">#6860</a>
            </td>
            <td>
                <b>
                    Remove develop prelease workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Creates noise in release notifications, can use "build from source" alternatives
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 08:15:57 +0000 UTC
    </div>
</div>

