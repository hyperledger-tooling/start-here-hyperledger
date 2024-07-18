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
                PR <a href="https://github.com/hyperledger/besu/pull/7352" class=".btn">#7352</a>
            </td>
            <td>
                <b>
                    Add metrics for trie log pruner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Add 3 counters, can be referenced in grafana with:
besu_pruner_trie_log_added_to_prune_queue_total
besu_pruner_trie_log_pruned_from_queue_total
besu_pruner_trie_log_pruned_trie_log_pruned_orphan_total

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
        Created At 2024-07-18 09:38:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7350" class=".btn">#7350</a>
            </td>
            <td>
                <b>
                    Optimise TrieLogPruner.preload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These optimisations only seem to save <= 17% of the time.

Control node took ~6mins.
Test node took between 5 mins and 5 mins 30 seconds on a couple of runs.

---

The problem with https://github.com/hyperledger/besu/pull/7337 is that for the duration of the async load, block import time appears to be affected. This could lead to impaired attestation performance and a missed proposal (although admittedly better than the alternative of downtime).

Ultimately need another PR that used a reasonable timeout for this load+prune operation, maybe 30 seconds.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 07:30:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7349" class=".btn">#7349</a>
            </td>
            <td>
                <b>
                    f --compatibility-eth64-forkid-enabled is set to true and there are no forks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This fixes an NPR that was thrown when no forks are configured and --compatibility-eth64-forkid-enabled is set to true.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 04:16:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7341" class=".btn">#7341</a>
            </td>
            <td>
                <b>
                    Dagger controller tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Demonstrates how to use Dagger to compose BesuControllers for use in privacy tests.

- Separate out flex group privacy test since it requires differently configured dependencies.
- test specific, inline module/component definitions
- reusable module for providing mockable enclaves, besu commands, and genesis

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 14:44:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7340" class=".btn">#7340</a>
            </td>
            <td>
                <b>
                    Use besu-untuned to execute the acceptance tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Use besu-untuned to execute different tests that need to run a besu node in a different process.
Also, there is no need to apply the JVM tuning related to GC and continuous profiling to this kind of tests.

<img width="1699" alt="image" src="https://github.com/user-attachments/assets/177d58c0-1a10-43e5-8ef0-2a1b29822ee7">


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


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 14:04:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7339" class=".btn">#7339</a>
            </td>
            <td>
                <b>
                    [minor] Remove redundant info from plugin summary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">plugins</span><span class="chip">ux</span>
            </td>
            <td>
                ## PR description
Some minor improvements to plugin summary:
- remove `Detected but not registered`
- remove the `Version` and duplicated v

Before:

```
# Plugin Registration Summary:                                                                     #
# Registered Plugins:                                                                              #
#  - ZkTrieLogPlugin (Version: besu-shomei-plugin/vv0.3.1)                                         #
# Skipped Plugins:                                                                                 #
#  - LineaExtraDataPlugin (Detected but not registered)                                            #
#  - LineaEndpointServicePlugin (Detected but not registered)                                      #
#  - LineaTransactionPoolValidatorPlugin (Detected but not registered)                             #
#  - LineaTransactionSelectorPlugin (Detected but not registered)                                  #
#  - BesuShomeiRpcPlugin (Detected but not registered)                                             #
#  - ContinuousTracingPlugin (Detected but not registered)                                         #
#  - CaptureEndpointServicePlugin (Detected but not registered)                                    #
#  - CountersEndpointServicePlugin (Detected but not registered)                                   #
#  - TracesEndpointServicePlugin (Detected but not registered)                                     #
# TOTAL = 1 of 10 plugins successfully registered.   

```
After

```
# Plugin Registration Summary:                                                                     #
# Registered Plugins:                                                                              #
#  - ZkTrieLogPlugin (besu-shomei-plugin/v0.3.1)                                                   #
# Detected but not registered:                                                                     #
#  - LineaExtraDataPlugin (linea-sequencer/v0.1.5-rc2)                                             #
#  - LineaEndpointServicePlugin (linea-sequencer/v0.1.5-rc2)                                       #
#  - LineaTransactionPoolValidatorPlugin (linea-sequencer/v0.1.5-rc2)                              #
#  - LineaTransactionSelectorPlugin (linea-sequencer/v0.1.5-rc2)                                   #
#  - BesuShomeiRpcPlugin (besu-shomei-plugin/v0.3.1)                                               #
#  - ContinuousTracingPlugin (linea-arithmetization/v0.1.5-rc6)                                    #
#  - CaptureEndpointServicePlugin (linea-arithmetization/v0.1.5-rc6)                               #
#  - CountersEndpointServicePlugin (linea-arithmetization/v0.1.5-rc6)                              #
#  - TracesEndpointServicePlugin (linea-arithmetization/v0.1.5-rc6)  
```


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 09:31:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7337" class=".btn">#7337</a>
            </td>
            <td>
                <b>
                    Make TrieLogPruner.preload async
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Simon Dudley <simon.dudley@consensys.net>

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Fixes #7322

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
        Created At 2024-07-17 05:42:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7336" class=".btn">#7336</a>
            </td>
            <td>
                <b>
                    Refactor - eliminate non-constant string concatenation from debug and trace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span>
            </td>
            <td>
                ## PR description
use atDebug() and atTrace()


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
        Created At 2024-07-17 04:38:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7333" class=".btn">#7333</a>
            </td>
            <td>
                <b>
                    Refactor - replace uses of QbftContext with BftContext
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
QbftContext wasn't adding anything extra any more since #7310 

Refs #7163 


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
        Created At 2024-07-17 00:39:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7331" class=".btn">#7331</a>
            </td>
            <td>
                <b>
                    Fix and restore disabled block creation unit tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Disabled block creation unit tests have been updated and fixed and re-enabled, this required to rework the `ExecutionContextTestFixture` to accept the genesis file to use, instead of using an hard-coded one as before, and for this there are more file changed/added

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #6850

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
        Created At 2024-07-16 09:30:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7330" class=".btn">#7330</a>
            </td>
            <td>
                <b>
                    Stop transaction selection on `TX_EVALUATION_TOO_LONG`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

we can safely stop transaction selection for block creation after a `TX_EVALUATION_TOO_LONG`, since it means that the tx took more that the block selection timeout to evaluate, and so does not make sense to continue the evaluation.

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
        Created At 2024-07-16 08:25:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7329" class=".btn">#7329</a>
            </td>
            <td>
                <b>
                    Update release checklist
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Takes into account latest changes from @cdivitotawela 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-16 07:35:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7328" class=".btn">#7328</a>
            </td>
            <td>
                <b>
                    adjust text so it succeeds on macOS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                ## PR description
LoggingTest AT failing on Mac because of weird separators

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
        Created At 2024-07-16 02:17:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7327" class=".btn">#7327</a>
            </td>
            <td>
                <b>
                    exclude permissioning test from default ATs run on PRs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">flake</span>
            </td>
            <td>
                ## PR description
Rather than disabling permissioning tests one by one as they flake, exclude them from being run on PRs.

Could run the permissioning suite on a nightly/weekly cadence instead

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
        Created At 2024-07-16 02:13:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7323" class=".btn">#7323</a>
            </td>
            <td>
                <b>
                    fix: eth_call JSON deserialization when unknown fields use hex encoded string values
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
fix: `eth_call` JSON deserialization when unknown fields use hex encoded string values that caused a runtime exception. `JsonCallParameter` deserialization logic is changed from `@JsonCreator` to `@JsonDeserialize(builder = JsonCallParameter.JsonCallParameterBuilder.class)` by introducing an inner builder. This fixed the issue where the Jackson's default integer to string coercion was applied for unknown parameters in the transaction object in `eth_call` when they specify hex encoded literals, for example: `"unknownField": "0xff"`.   

This fix will allow Besu's `eth_call` to match Geth's `eth_call` behaviour to ignore unknown values in the transaction object of `eth_call`'s JSON.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes https://github.com/hyperledger/besu/issues/7294

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
        Created At 2024-07-15 09:16:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7321" class=".btn">#7321</a>
            </td>
            <td>
                <b>
                    Reduce trie log pruning window size and add startup log
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
        Created At 2024-07-15 03:38:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7320" class=".btn">#7320</a>
            </td>
            <td>
                <b>
                    6612 update changelog with removed syncmodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Update changelog as requested in https://github.com/hyperledger/besu/pull/7309
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
https://github.com/hyperledger/besu/issues/6612

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-14 23:07:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7319" class=".btn">#7319</a>
            </td>
            <td>
                <b>
                    Update datacopy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Check for OOG earlier in DataCopy.
Add unit tests to cover operation branches.

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
        Created At 2024-07-13 19:32:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7317" class=".btn">#7317</a>
            </td>
            <td>
                <b>
                    Update unit test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

* Update parameterized unit tests so the enumerate with --dry-run
* Update the prague-withdrawal.json unit test to handle current code

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
        Created At 2024-07-12 21:18:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7316" class=".btn">#7316</a>
            </td>
            <td>
                <b>
                    Feature/use gnark-crypto for eip-2537
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Use gnark-crypto for eip-2537, decomposed from #7262 to compartmentalize


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
        Created At 2024-07-12 20:07:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7315" class=".btn">#7315</a>
            </td>
            <td>
                <b>
                    Test template refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add a package namespace replacement parameter to the spec test templating function.  This allows us to ensure we have the correct namespace for the generated class and the target filesystem (ensures they run), and allows us to remove duplicated templates that differed only by the namespace they were generating for.

* DRY up test tempates
* ensure all execution-spec tests are running
* bump besu-native dep to 0.9.2

Motivation: this was originally part of #7262, decomposed here as a standalone PR


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
        Created At 2024-07-12 17:07:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7314" class=".btn">#7314</a>
            </td>
            <td>
                <b>
                    Add new PoA network option to use bootnodes during any peer table refresh, not just the first one
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR adds the option in PoA networks only to query the bootnodes whenever the peer table is being refreshed.

The behaviour today is that the bootnodes are queried on first startup, but if no peers are found on that occasion Besu will not use the bootnode again until it is restarted.

The new option is `on` by default. Setting `--poa-discovery-retry-bootnodes` disables it.

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-12 16:56:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7313" class=".btn">#7313</a>
            </td>
            <td>
                <b>
                    Make maintained PoA bootnode connections configurable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR follows on from https://github.com/hyperledger/besu/pull/7257. Specifically it makes the behaviour configurable and defaults to `off`. Since the `25.7.0` release has just gone out this PR will technically be a change in behaviour, so I'll add a change log entry accordingly. However, assuming this PR is included in an upcoming release I don't imagine any users will be affected by the behaviour change.

In an enterprise network with a large number of nodes, maintaining connections to the bootnodes could be problematic for the bootnodes. Defaulting the behaviour to `off` avoids the need to specifically disable the behaviour on all of the nodes, but allows a smaller chain to be configured to still treat bootnodes like static nodes.

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-12 15:54:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7312" class=".btn">#7312</a>
            </td>
            <td>
                <b>
                    Improve blob size transaction selector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

The main goal of this PR is to make clearer the reason a blob tx is not selected during block creation, with the introduction of 2 specifics not selected results:

- BLOBS_FULL = The block already contains the max number of allowed blobs.
- TX_TOO_LARGE_FOR_REMAINING_DATA_GAS = The transaction has not been selected since there is not enough remaining data gas in the block to fit the blobs of the tx.

and to achieve that it was clearer to extract the blob tx selection login in its own class `BlobSizeTransactionSelector`, while doing that a small bug was fixed, since data gas used was added to gas used when computing if a block was full, while these 2 gas types are independent, [see here for details](https://github.com/hyperledger/besu/pull/7312/files#r1677540274).

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
        Created At 2024-07-12 15:45:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7310" class=".btn">#7310</a>
            </td>
            <td>
                <b>
                    removed PKI backed QBFT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
fixes #7163


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
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
        Created At 2024-07-12 06:57:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7309" class=".btn">#7309</a>
            </td>
            <td>
                <b>
                    6612: Remove deprecated sync modes and related helper methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
Remove deprecated sync modes and related helper methods

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
https://github.com/hyperledger/besu/issues/6612

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
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
        Created At 2024-07-12 05:02:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7308" class=".btn">#7308</a>
            </td>
            <td>
                <b>
                    disable flaky test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">flake</span>
            </td>
            <td>
                ## PR description


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
        Created At 2024-07-12 04:12:06 +0000 UTC
    </div>
</div>

