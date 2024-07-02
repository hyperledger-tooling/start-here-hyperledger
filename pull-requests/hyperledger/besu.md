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

