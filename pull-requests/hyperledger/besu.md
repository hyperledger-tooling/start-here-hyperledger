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
                PR <a href="https://github.com/hyperledger/besu/pull/7266" class=".btn">#7266</a>
            </td>
            <td>
                <b>
                    add consolidation request type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
A new consolidation request type: https://eips.ethereum.org/EIPS/eip-7251#consolidation-request

## Fixed Issue(s)
refs #7254 


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
        Created At 2024-06-26 09:12:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7264" class=".btn">#7264</a>
            </td>
            <td>
                <b>
                    Snapserver GetTrieNodes request to handle short hash for storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Allows snapsync server to GetTrieNodes request for storage to handle a hash with less than 32 bytes. It's not mentioned in the snap sync spec but Geth handles such requests and the hive tests rely on this behaviour. Implementing this fixes a hive test case.

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
        Created At 2024-06-26 05:17:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7263" class=".btn">#7263</a>
            </td>
            <td>
                <b>
                    Implement System Calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">Prague</span>
            </td>
            <td>
                ## PR description

- Introduces system calls -  ( a call to `CONTRACT_ADDRESS` as `SYSTEM_ADDRESS`). This is a system operation and therefore:
  - the call must be executed to completion
  - the call does not count against the block’s gas limit
  - the call does not follow the [EIP-1559](https://eips.ethereum.org/EIPS/eip-1559) burn semantics - no value should be transferred as part of the call
  - if no code exists at CONTRACT_ADDRESS, the call must fail silently

- Changes `withdrawalRequestProcessor` to perform a `system call` instead of directly manipulating storage. 

## Fixed Issue(s)
fixes #6918 
fixes #7259


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-25 23:59:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7262" class=".btn">#7262</a>
            </td>
            <td>
                <b>
                    Feature/use gnark-crypto for ecc precompiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Use gnark-crypto from besu-native for ECC precompiles
* eip-2537
* eip-196
* eip-197

This will get besu onto a supported and more performant ECC library, and should allow us to remove tech debt in besu-native.

This PR also addresses some templating problems that exist with some of the execution spec tests, where tests are created in directories that do not match their namespace (and thus were not being run)


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
        Created At 2024-06-25 23:01:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7258" class=".btn">#7258</a>
            </td>
            <td>
                <b>
                    Implement getNearest methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Add getNearestAfter method needed for verkle and fix getNearestBefore method


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
        Created At 2024-06-25 08:50:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7257" class=".btn">#7257</a>
            </td>
            <td>
                <b>
                    Add bootnodes to the maintained peer list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">peering</span>
            </td>
            <td>
                ## PR description
This PR adds the bootnodes to the maintained-peer list in a permissioned chain. Currently the maintained node list only contains static nodes and nodes added with `admin_addPeer`. Adding bootnodes to the maintained list ensures that if a bootnode is offline when the node starts, it will retry its connection once a minute rather than requiring a restart.

Bootnode connectivity in a public-chain node remains unchanged.

## Fixed issues
Fixes https://github.com/hyperledger/besu/issues/7261

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] ~For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests~

Based on the outcome of this PR, I plan to raise a docs PR to describe how connections are maintained to bootnodes and static nodes since there isn't much detail covering the behaviour today. I'll wait for the outcome of this PR before raising the docs changes though.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-25 08:20:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7256" class=".btn">#7256</a>
            </td>
            <td>
                <b>
                    Disable Flaky tests - permissioning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">flake</span><span class="chip">permissioning</span>
            </td>
            <td>
                ## PR description
Disabled a number of flaky permissioning tests
Also corrected name of this test method `shouldNotIgnoreSenderBalanceAccountWhenStrictModeEnabled`. 

## Fixed Issue(s)
fixes #7191 
fixes #7151 


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
        Created At 2024-06-25 02:44:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7253" class=".btn">#7253</a>
            </td>
            <td>
                <b>
                    update to work with the new max retries value
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
        Created At 2024-06-24 15:06:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7252" class=".btn">#7252</a>
            </td>
            <td>
                <b>
                    Fix the wrong 'Identifier' and 'Synchronizer' usage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix the wrong 'Identifier' and 'Synchronizer' usage

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-22 19:01:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7251" class=".btn">#7251</a>
            </td>
            <td>
                <b>
                    Update Docker base image to Ubuntu 24.04
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
        Created At 2024-06-21 17:23:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7249" class=".btn">#7249</a>
            </td>
            <td>
                <b>
                    Fix flaky SECP256R1 test
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
        Created At 2024-06-21 14:24:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7248" class=".btn">#7248</a>
            </td>
            <td>
                <b>
                    Refactoring - Group P2P options into its own class
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
        Created At 2024-06-20 23:51:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7247" class=".btn">#7247</a>
            </td>
            <td>
                <b>
                    Remove deprecation message for `--Xp2p-peer-lower-bound`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Remove the deprecation message for `--Xp2p-peer-lower-bound`. This option has already been removed. 
See https://github.com/hyperledger/besu/pull/6501
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-20 09:43:14 +0000 UTC
    </div>
</div>

