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

A small change was required to update Vert.x, since in the new version the CORS check have changed, and if using `.*` to match any origin, the origin must have as protocol one of: `http`, `https` or `ftp`, but since we also want to support browser extensions as origins, which have protocols like `moz-extension://` , then the regex should be written has `.*://.*`  

[In the version websocket write handlers are disabled by default](https://github.com/eclipse-vertx/vert.x/issues/4625), and since we use them, we need to enable them.

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

