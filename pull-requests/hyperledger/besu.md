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
                PR <a href="https://github.com/hyperledger/besu/pull/6895" class=".btn">#6895</a>
            </td>
            <td>
                <b>
                    add rlp decode subcommand
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
Adds `decode` subcommand to rlp based on this [Issue](https://github.com/hyperledger/besu/issues/3074)

Example
```
besu rlp decode --from=<input-file> --to=<output-file> --type=<IBFT_EXTRA_DATA|QBFT_EXTRA_DATA>
```

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
        Created At 2024-04-06 23:05:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6894" class=".btn">#6894</a>
            </td>
            <td>
                <b>
                    Default bonsai to fully flat db and code storage by codehash 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
defaults bonsai to fully flattened db
deprecates snap sync full flat config param
creates --Xbonsai-full-flat-db-enabled parameter
FlatDbStrategyProvider defers config if db is empty and persists a flat db strategy config

Draft while sorting out 2 cli param unit tests


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
        Created At 2024-04-06 05:02:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6893" class=".btn">#6893</a>
            </td>
            <td>
                <b>
                    Docker develop publishing task
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add a minimal github action to publish `develop` docker containers on merge to main.  

The task will publish each variant and arch as a develop image, and publish a multi-arch image for each variant.
e.g. the images that this task will publish on every merge to main (currently) are:

multi-arch variants
* develop 
* develop-openjdk-latest
* develop-graalvm
* develop-openj9-jdk-17
* develop-openjdk-17-debug 
* develop-openjdk-17 

arch-variants:
* develop-arm64 
* develop-openjdk-latest-arm64
* develop-graalvm-arm64
* develop-openj9-jdk-17-arm64
* develop-openjdk-17-debug-arm64
* develop-openjdk-17-arm64
* develop-amd64
* develop-openjdk-latest-amd64
* develop-graalvm-amd64
* develop-openj9-jdk-17-amd64
* develop-openjdk-17-debug-amd64
* develop-openjdk-17-amd64


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
        Created At 2024-04-06 00:10:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6892" class=".btn">#6892</a>
            </td>
            <td>
                <b>
                    fix:Issue #2639 -> Improve warning on invalid JDK version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Ensure compatible JDK version is installed and used by adding "org.kordamp.gradle.enforcer" gradle plugin and a RequireJavaVersion rule. Gradle enforcer is a port of the maven enforcer plugin.

## Fixed Issue(s)
Fixes #2639 

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

I just checked unit tests as the PR does not modify the code.
By the way, note that KweiTest is environment-dependent. Decimal separator is not "." on all systems :)

- [x] unit tests: `./gradlew build`
- [] acceptance tests: `./gradlew acceptanceTest`
- [] integration tests: `./gradlew integrationTest`
- [] reference tests: `./gradlew ethereum:referenceTests:referenceTests`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-05 22:09:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6890" class=".btn">#6890</a>
            </td>
            <td>
                <b>
                     Correctly initialize the txpool as disabled on creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Correctly initialize the txpool as disabled on creation, to avoid exception when calling txpool methods before the initial sync phase is done.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #6863 

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
        Created At 2024-04-05 10:23:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6889" class=".btn">#6889</a>
            </td>
            <td>
                <b>
                    confirm pivot block - removed requirement for chain height estimate 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
When choosing the "best" peer to try to confirm the pivot block
* use the default comparator (TTD then chain height)
* remove the pre-requirement for the chain height estimate 
* don't disconnect the "worst" useless peer at this point
* and update the peer's chain height estimate if the pivot block is confirmed

## Fixed Issue(s)
Fixes #6887 


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
        Created At 2024-04-05 10:08:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6886" class=".btn">#6886</a>
            </td>
            <td>
                <b>
                    Improve logging of peer disconnects due to subprotocol triggered
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add additional detail when we disconnect with SUBPROTOCOL_TRIGGERED disconnect reason. I've extended the enum with additional SUBPROTOCOL_TRIGGERED values using the same code `0x10` and added a message to these extended `SUBPROTOCOL_TRIGGERED` reasons.

If we receive a `0x10` this is mapped back to the generic `SUBPROTOCOL_TRIGGERED` reason.

example with the changes
```
Disconnecting connection 1859339149, peer 0x6b8a113cb2edfa5d... reason 0x10 SUBPROTOCOL_TRIGGERED_MISMATCHED_NETWORK Mismatched network id
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
        Created At 2024-04-05 05:38:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6885" class=".btn">#6885</a>
            </td>
            <td>
                <b>
                    Add debug logging to see why we stop downloading from peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Logging for debugging #6884 


Example when peer disconnected:
```
DEBUG | FastSyncDownloadPipelineFactory | Stopping chain download due to disconnected peer PeerId: 0x143e11fb766781d2... PeerReputation score: 150, timeouts: {}, useless: 4, validated? true, disconnected? true, client: Geth/v1.13.14-stable-2bd6bd01/linux-amd64/go1.21.7, [Connection with hashCode 68650968 inboundInitiated? false initAt 1712288750661], enode://143e11fb766781d22d92a2e33f8f104cddae4411a122295ed1fdb6638de96a6ce65f5b7c964ba3763bba27961738fef7d3ecc739268f3e5e771fb4c87b6234ba@146.190.1.103:30303
```

Example when lastRoundHeader >= pivotBlockHeader:
```
DEBUG | FastSyncDownloadPipelineFactory | Stopping chain download as lastRoundHeader=1283816 is not less than pivotBlockHeader=1283816 for peer PeerId: 0x7a52e545cdc62aea... PeerReputation score: 150, timeouts: {}, useless: 0, validated? true, disconnected? false, client: besu/v24.3.0/linux-x86_64/openjdk-java-17, [Connection with hashCode 1511026419 inboundInitiated? true initAt 1712291178516], enode://7a52e545cdc62aea505e6f8795b10741ba7a9ef4b7daba88af55c0bd5af74ebeefe1098faeb31fea320f2c00297cfc5ad5af6c94916ce6b5d4f05e2d8b1ad562@202.61.198.135:30303?discport=0
```


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-05 01:52:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6883" class=".btn">#6883</a>
            </td>
            <td>
                <b>
                    EIP-7002: Validator Exit contract helper and adding exits to created blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                _Sorry for the big PR! I tried to keep it more concise but lots of the pieces kinda work together so it was hard to separate them! Hopefully it isn't too bad to review as a bulk of the changes are adding a parameter to a constructor or something like that..._ ❤️ 

This is a preliminary implementation of [EIP-7002](https://eips.ethereum.org/EIPS/eip-7002) logic for adding exits from the Validator Exit smart contract into blocks (and including them on the execution payload object of the Engine API).

**Summary of changes**
- Updated engine API method and ExeutionPayload structure to support exits
- Implemented Validator Exit Contract Helper
- Updated BlockCreator to include exits from the validator exit contract

fixes #6881 and #6882

**Open Questions/Future Improvements**
- Do we need extra validation on `AbstractBlockProcessor` (e.g. check that we do not have more exits than expected). I have a feeling we do not need to as we are running the system logic as part of processing, so any difference between the exits in the block we are validating would be caught by a different exits_root post our processing. But I might be wrong. The same question applies to `MainnetBlockBodyValidator. validateBodyLight()`.
- The Validator Exits contract address might need to be parameterized for each network. The same applies to things like the maximum number of exits per block, etc.
- Do we need to have `ValidatorExitContractHelper` behind a protocol schedule setup in case the contract goes through some changes in future upgrades?

## Engine API changes

Most of the logic was already there, few pieces had to be added (e.g. constructor parameters but the core of the logic hasn't changed). The more important change is how GetPayloadV4 includes the exits in the execution payload.

## Validator Exit Contract Helper

This is an initial implementation based on the work done by lightclient on the Validator Exit smart contract (https://github.com/lightclient/7002asm), and also using the bytecode defined in the EIP (https://eips.ethereum.org/EIPS/eip-7002#deployment).

Each exit uses 3 storage slots (each slot has 32 bytes). There is a bit of trickery to ensure they fit in exactly on 3 slots (some right/left padding depending on the field). The detailed diagram of the expected storage can be seen [in this code](https://github.com/lightclient/7002asm/blob/main/src/main.eas#L239-L251).

## Including exits on blocks

The system call logic has been implemented in a way that manipulates the contract storage as if we were executing the call through the EVM (although no EVM is involved). This seems to be the expected behaviour for system calls. The heard of this is how `AbstractBlockCreator` uses `ValidatorExitContractHelper.popExitsFromQueue(..)`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-04 21:09:30 +0000 UTC
    </div>
</div>

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
                PR <a href="https://github.com/hyperledger/besu/pull/6868" class=".btn">#6868</a>
            </td>
            <td>
                <b>
                    [MINOR] add toString for handshake messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span><span class="chip">peering</span>
            </td>
            <td>
                ## PR description
Before -
`
{"@timestamp":"2024-04-03T04:03:50,365","level":"TRACE","thread":"nioEventLoopGroup-3-10","class":"ECIESHandshaker","message":"First ECIES handshake message under INITIATOR role: org.hyperledger.besu.ethereum.p2p.rlpx.handshake.ecies.InitiatorHandshakeMessageV4@2a66bbb5","throwable":""}
`

After -
`
{"@timestamp":"2024-04-03T04:03:50,925","level":"TRACE","thread":"nioEventLoopGroup-3-1","class":"ECIESHandshaker","message":"Received responder's ECIES handshake message from node 0xb2aaeccb38b380e6663458bf7066f132...: ResponderHandshakeMessageV4{ephPublicKey=0xe8afcfe96360bb7e83a223d5b0b080a9b7157db5edfda2dfbadcb057c512dacd3718a538a64afa41e2e5fbcc929154bedd861619f72ca413ecabe8f8e0678bf6, nonce=0xb4235af56982f5f348bb762625da18a775a977053b0e4bfec9546e3b6abc9858}","throwable":""}
`
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
        Created At 2024-04-03 04:11:54 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6858" class=".btn">#6858</a>
            </td>
            <td>
                <b>
                    [MINOR] Use 7 chars instead of 10 for source build hash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Think 7 is the standard length...at least it matches what's in https://github.com/hyperledger/besu/commits/main/ which makes cross referencing a deployment to a commit easier.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 03:06:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6857" class=".btn">#6857</a>
            </td>
            <td>
                <b>
                    build: Remove incomplete artifactory task
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
build: Remove incomplete artifactory task. The top level artifactory task was used to upload dists to artifactory which has been moved to GH

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


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
        Created At 2024-04-02 01:37:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6856" class=".btn">#6856</a>
            </td>
            <td>
                <b>
                    workaround for broken publishing of buildinfo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The 24.4.0 release deployed artifacts to artifactory as expected, but failed when updating the build-info, which was a surprise. This is a workaround which disables that publishing temporarily, and also defers jar publishing till the end of the workflow, to avoid derailing more important steps.


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 17:08:56 +0000 UTC
    </div>
</div>

