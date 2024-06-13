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
                PR <a href="https://github.com/hyperledger/besu/pull/7223" class=".btn">#7223</a>
            </td>
            <td>
                <b>
                    feat: Add network option for LUKSO Mainnet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This PR provides an option to connect to [LUKSO Mainnet](https://www.lukso.network/) network, using `--network=lukso` flag.

## Fixed Issue(s)

No matching issues 

### Thanks for sending a pull request! Have you done the following?

- [X] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [X] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [X] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 09:24:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7222" class=".btn">#7222</a>
            </td>
            <td>
                <b>
                    Add build version option to prefix git hash with custom version property
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Adds the option to provide a custom version prefix at build time that will be prefixed to the git hash. Currently a custom version can't include the githash. This follows on from some recent version refactoring in https://github.com/hyperledger/besu/pull/6699

Specifically it allows for `-Pversionprefix=24.5.2` to result in a version like `v24.5.2-16ff080`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 09:04:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7221" class=".btn">#7221</a>
            </td>
            <td>
                <b>
                    Handle invalid snap getTrieNode requests with empty paths gracefully
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Handle invalid requests with empty paths for GetTrieNode snapsync server requests more gracefully and return an empty response instead of throwing an `ArrayIndexOutOfBoundsException`, catching this and returning an empty response.

In the snapsync server handling of `GetTrieNodes` message we are assuming that there is at least one path in the request. When there is an invalid request with no paths we fail with an `ArrayIndexOutOfBoundsException`.

```
2024-06-12 03:26:15.257+00:00 | nioEventLoopGroup-3-9 | ERROR | SnapServer | Unexpected exception serving trienodes request
java.lang.ArrayIndexOutOfBoundsException: Index 0 out of bounds for length 0
	at java.base/java.util.ImmutableCollections$ListN.get(ImmutableCollections.java:687)
	at org.hyperledger.besu.ethereum.eth.manager.snap.SnapServer.lambda$constructGetTrieNodesResponse$23(SnapServer.java:549)
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
        Created At 2024-06-13 00:41:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7219" class=".btn">#7219</a>
            </td>
            <td>
                <b>
                    Revert "Update Dockerfile - reuse NO_PROXY_CACHE env (#7203)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit dfe256e6478a91122e40adda928a71e1353668f1.
Reverts https://github.com/hyperledger/besu/pull/7203

There's an issue running docker develop workflow

https://github.com/hyperledger/besu/actions/runs/9491467523

```
Run docker run --rm -i hadolint/hadolint < docker/Dockerfile
Unable to find image 'hadolint/hadolint:latest' locally
latest: Pulling from hadolint/hadolint
db4123164570: Pulling fs layer
db4123164570: Download complete
db4123164570: Pull complete
Digest: sha256:fff226bdf9ebcc08db47fb90ee144dd770120b35c2b1cbbb46e932a650cfe232
Status: Downloaded newer image for hadolint/hadolint:latest
-:7 DL3008 warning: Pin versions in apt get install. Instead of `apt-get install <package>` use `apt-get install <package>=<version>`
Error: Process completed with exit code 1.
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
        Created At 2024-06-13 00:25:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7216" class=".btn">#7216</a>
            </td>
            <td>
                <b>
                    Add container security scanning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Container security scanning workflow added. This runs on schedule everyday. Also possible to run on-demand for a given image tag. This replace the CircleCI job running container scan daily. Schedule job only runs for the tag `develop`.

## Fixed Issue(s)
fixes #7154

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
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
        Created At 2024-06-13 00:04:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7215" class=".btn">#7215</a>
            </td>
            <td>
                <b>
                    chore: fix some comments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

fix some comments

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
        Created At 2024-06-12 15:31:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7214" class=".btn">#7214</a>
            </td>
            <td>
                <b>
                    check correctly the storage in ToyAccount
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

We are not correctly checking the storage in the ToyAccount for the isStorageEmpty method. It can create issue during the contract creation step when we check if an account exist or not (only a problem for the toy environment and not a problem for mainnet). 

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
        Created At 2024-06-12 14:09:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7213" class=".btn">#7213</a>
            </td>
            <td>
                <b>
                    [VERKLE] Fix unit tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Fix build and unit tests on verkle branch 

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
        Created At 2024-06-12 08:09:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7212" class=".btn">#7212</a>
            </td>
            <td>
                <b>
                    changed arm runner
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
        Created At 2024-06-12 05:37:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7211" class=".btn">#7211</a>
            </td>
            <td>
                <b>
                    disable flaky test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
disable flaky permissioning tests

## Fixed Issue(s)
fixes #7108 
fixes #7155 


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
        Created At 2024-06-12 04:36:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7210" class=".btn">#7210</a>
            </td>
            <td>
                <b>
                    hotfix: update module checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
0.8.4 besu-native artifacts were inadvertently re-published. This hotfix is required to be able to build from source with those artifacts. 

## Fixed Issue(s)
fixes #7170


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
        Created At 2024-06-12 01:57:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7209" class=".btn">#7209</a>
            </td>
            <td>
                <b>
                    Updated EIP-7002 WithdrawalRequestV1 field (validatorPublicKey -> validatorPubkey)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Updated WithdrawalRequestV1 field according to https://github.com/ethereum/execution-apis/pull/549.

(validatorPublicKey -> validatorPubkey)

This will soon be updated in Teku as well (https://github.com/Consensys/teku/issues/8359)

## Fixed Issue(s)
N/A


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-11 23:51:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7208" class=".btn">#7208</a>
            </td>
            <td>
                <b>
                    Remove EIP-3074 code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Remove all EIP-3074 code from Besu. Since EIP-3074 has been replaced
with EIP-7702 in Pectra, and there is no intent to schedule it for a
future fork there is no need to retain the code.

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
        Created At 2024-06-11 19:02:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7207" class=".btn">#7207</a>
            </td>
            <td>
                <b>
                    Issue Template for Release managers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

new template for creating an issue to track Release action items.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-11 15:24:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7206" class=".btn">#7206</a>
            </td>
            <td>
                <b>
                    [VERKLE] Preload triekeys 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Currently, trie keys generation will gather all transactions data and generate a single large batch of trie keys at once.
However, there are already mechanisms implemented in Besu to preload those trie keys in a background thread during block processing. 

This PR generates the different triekeys in the background in order to have a maximum of triekeys already calculated at the end of the block

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
        Created At 2024-06-11 13:03:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7204" class=".btn">#7204</a>
            </td>
            <td>
                <b>
                    Don't persist BFT proposed blocks, only committed ones
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR changes BFT block proposal validation to not persist the changes as a result of the proposed block. When a QBFT `commit` message or Ethereum `NewBlock` message is processed the changes will still be persisted at that point.

Prior to this PR I could only get a few 1000 transactions through a 4-validator QBFT chain before I hit `Invalid block` error. With this fix in place I can run any number of high TPS tests against a 4-validator chain and have yet to see an `Invalid block` error.

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/6680

(It might fix this issue, or there could still be something to resolve regarding the `RocksDB busy` error. I suspect this PR will improve the above issue at the very least, but suggest closing it with this PR and re-opening if it still occurs after this has merged)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-11 10:40:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7203" class=".btn">#7203</a>
            </td>
            <td>
                <b>
                    Update Dockerfile - reuse NO_PROXY_CACHE env
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Just noticed this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-11 10:01:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7202" class=".btn">#7202</a>
            </td>
            <td>
                <b>
                    disable flaky test - DNSDaemon periodic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Disable this test since it's blocking PRs

## Fixed Issue(s)
refs #7201 


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
        Created At 2024-06-11 07:14:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7200" class=".btn">#7200</a>
            </td>
            <td>
                <b>
                    fix(test): Fix dns daemon periodic test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
fix(test): Fix dns daemon periodic test. Increase second run to 3 seconds

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
        Created At 2024-06-11 05:56:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7199" class=".btn">#7199</a>
            </td>
            <td>
                <b>
                    Update gradle to 8.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Update gradle to 8.8

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
        Created At 2024-06-11 04:32:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7198" class=".btn">#7198</a>
            </td>
            <td>
                <b>
                    Update changelog for 24.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Update changelog for 24.6.0 release

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
        Created At 2024-06-11 03:16:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7194" class=".btn">#7194</a>
            </td>
            <td>
                <b>
                    Support for eth_maxPriorityFeePerGasPrice
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #5658 

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-09 14:14:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7193" class=".btn">#7193</a>
            </td>
            <td>
                <b>
                    Promote --bonsai-limit-trie-logs-enabled to stable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also --bonsai-trie-logs-pruning-window-size

Following https://github.com/hyperledger/besu/pull/7181 and https://github.com/hyperledger/besu/pull/7192

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-07 13:38:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7192" class=".btn">#7192</a>
            </td>
            <td>
                <b>
                    Promote option - bonsai-limit-trie-logs-enabled and bonsai-trie-logs-pruning-window-size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Create --bonsai-limit-trie-logs-enabled as alias of --Xbonsai-limit-trie-logs-enabled and unhide option
Same for bonsai-trie-logs-pruning-window-size

Remove --bonsai-historical-block-limit=512 from minimalist_staker profile so it inherits the default which is the same value

Follow on from #7181 
Will restructure code from Unstable -> Stable in next PR.

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-07 06:44:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7190" class=".btn">#7190</a>
            </td>
            <td>
                <b>
                    Snapserver responses to return at least one response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
The snap server responses must return at least one response item if the data can be retrieved according to the spec https://github.com/ethereum/devp2p/blob/master/caps/snap.md. This applies to all the request types.

After making this change all the GetByteCodes hive tests are passing. Note still need to make a change to hive testsuite to enable snapserver before this will be seen.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Part of #7197

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
        Created At 2024-06-07 05:55:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7189" class=".btn">#7189</a>
            </td>
            <td>
                <b>
                    feat: Refactor Node DNS Resolver to use vertx virtual threads
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Refactor Node DNS Resolver to use vertx virtual threads (Java 21).
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
        Created At 2024-06-07 04:37:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7188" class=".btn">#7188</a>
            </td>
            <td>
                <b>
                    Move traceEndTransaction after coinbase refund, add self destruct set to the method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Fix for traceEndTransaction not considering the coinbase refund, added self destruct set

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 13:55:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7187" class=".btn">#7187</a>
            </td>
            <td>
                <b>
                    Fix: always use miningParametersSupplier
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

#7102 introduced a regression that broke the `ethereum_min_gas_price` and `ethereum_min_priority_fee metrics`, since `miningParameters` where created twice, instead of always use the `miningParametersSupplier`

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
        Created At 2024-06-06 13:31:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7186" class=".btn">#7186</a>
            </td>
            <td>
                <b>
                    In enterprise profile, use sync-mode=FULL and data-storage-format=FOREST
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Also remove lower casing of profile names to keep CLI string values consistent with other options

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 13:12:35 +0000 UTC
    </div>
</div>

