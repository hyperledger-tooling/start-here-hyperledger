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
                PR <a href="https://github.com/hyperledger/besu/pull/7397" class=".btn">#7397</a>
            </td>
            <td>
                <b>
                    Lock evmtool code-validate into runtime mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

To conform to fuzzing practices, `code-validate` expects all code to be
runtime code.

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
        Created At 2024-07-29 22:57:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7396" class=".btn">#7396</a>
            </td>
            <td>
                <b>
                    Change EOF Parsing to be non-recursive
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

EOF subcontainer parsing was recursive, potentially opening up stack
attacks. 
Replace subcontainer parsing with a flat iterative solution.

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
        Created At 2024-07-29 20:44:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7395" class=".btn">#7395</a>
            </td>
            <td>
                <b>
                    In process RPC service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Expose a way to call RPC method in process, so they can be invoked by plugins without the overhead of the network (or native socket) and the json (de)serialization.

The interface is still fragile, because RPC method inputs and outputs are not typed, but just Object, so a next step will be to make them typed so plugins will discover at compile time that something is broken, but that will be address in another PR.

Do not be scared by the amount of file changed since many are due to the move of some classes in the plugin-api module.

This feature is disabled by default and can be enabled setting the new experimental flag `Xin-process-rpc-enabled=true`, and to enabled specific RPC namespaces use the new experimental option `Xin-process-rpc-apis` with a comma separated list of namespaces.

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
        Created At 2024-07-29 16:48:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7394" class=".btn">#7394</a>
            </td>
            <td>
                <b>
                    7702 bugfixes for devnet-1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Process the authority list before increasing the sender nonce, make sure that the updated balance of the sender is calculated correctly if they sign an authorization as well

## Fixed Issue(s)
fixes #7391 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-29 13:50:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7393" class=".btn">#7393</a>
            </td>
            <td>
                <b>
                    Refactor TrieLogPruner preload timeout to be more testable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                An improved version of https://github.com/hyperledger/besu/pull/7365

Example of INFO level logging during timeout...
```
{"@timestamp":"2024-07-29T11:58:49,398","level":"INFO","thread":"main","class":"TrieLogPruner","message":"Trie log pruner queue preload starting...","throwable":""}
{"@timestamp":"2024-07-29T11:58:49,399","level":"INFO","thread":"main","class":"TrieLogPruner","message":"Attempting to load first 5000 trie logs from database...","throwable":""}
{"@timestamp":"2024-07-29T11:58:49,400","level":"INFO","thread":"main","class":"TrieLogPruner","message":"Trie log pruning will timeout after 30 seconds. If this is timing out, consider using `besu storage trie-log prune` subcommand, see https://besu.hyperledger.org/public-networks/how-to/bonsai-limit-trie-logs","throwable":""}
{"@timestamp":"2024-07-29T11:59:19,401","level":"WARN","thread":"main","class":"TrieLogPruner","message":"Timeout occurred while loading and processing 5000 trie logs from database","throwable":""}
{"@timestamp":"2024-07-29T11:59:19,437","level":"INFO","thread":"pool-8-thread-1","class":"TrieLogPruner","message":"Operation interrupted, but will attempt to prune what's in the queue so far...","throwable":""}
{"@timestamp":"2024-07-29T11:59:19,452","level":"INFO","thread":"pool-8-thread-1","class":"TrieLogPruner","message":"...pruned 412 trie logs","throwable":""}
{"@timestamp":"2024-07-29T11:59:19,452","level":"INFO","thread":"main","class":"TrieLogPruner","message":"Trie log pruner queue preload complete.","throwable":""}
```

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
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`

Signed-off-by: Simon Dudley <simon.dudley@consensys.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-29 12:01:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7392" class=".btn">#7392</a>
            </td>
            <td>
                <b>
                    Move `JsonRpcResponseType` to `RpcResponseType` in the plugin API module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This PR has is preparatory for PR https://github.com/hyperledger/besu/pull/7379/, to make the latter easier to review, there are no functional changes here, but just the move `JsonRpcResponseType` to `RpcResponseType` in the plugin API module.

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
        Created At 2024-07-29 10:56:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7390" class=".btn">#7390</a>
            </td>
            <td>
                <b>
                    Metrics for sync phases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR is adding metrics to the time for the chain download and for the world state download.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-29 06:20:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7388" class=".btn">#7388</a>
            </td>
            <td>
                <b>
                    fix(doc): tiny typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

just a tiny typo in a comment

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
        Created At 2024-07-28 15:40:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7386" class=".btn">#7386</a>
            </td>
            <td>
                <b>
                    Add world state to traceEndblock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Adds the world state to `traceEndBlock` in order to be able the state of the accounts after the whole block has been processed

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-26 15:01:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7385" class=".btn">#7385</a>
            </td>
            <td>
                <b>
                    Rotate changelog for 24.7.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of https://github.com/hyperledger/besu/issues/7384
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-26 06:36:18 +0000 UTC
    </div>
</div>

