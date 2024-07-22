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
                PR <a href="https://github.com/hyperledger/besu/pull/7357" class=".btn">#7357</a>
            </td>
            <td>
                <b>
                    Disable bonsai-limit-trie-logs-enabled if sync-mode=FULL
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since [bonsai-limit-trie-logs-enabled has been defaulted to true](https://github.com/hyperledger/besu/pull/7181), instead of preventing startup, implicitly set `bonsai-limit-trie-logs-enabled=false` and warn...

```
besu --sync-mode=FULL
...
2024-07-22 13:34:52.764+10:00 | main | WARN  | Besu | Cannot enable --bonsai-limit-trie-logs-enabled with --sync-mode FULL and --data-storage-format BONSAI. --bonsai-limit-trie-logs-enabled has been automatically disabled.
```

However, if you explicitly try to set it to true, you get a startup error...

```
besu --sync-mode=FULL --bonsai-limit-trie-logs-enabled=true
...
2024-07-22 14:56:11.189+10:00 | main | ERROR | Besu | Failed to start Besu
picocli.CommandLine$ParameterException: Cannot enable --bonsai-limit-trie-logs-enabled with --sync-mode FULL and --data-storage-format=BONSAI. You must set --bonsai-limit-trie-logs-enabled=false or use a different sync-mode
```

```
BESU_SYNC_MODE=FULL BESU_BONSAI_LIMIT_TRIE_LOGS_ENABLED=TRUE besu
...
2024-07-22 15:32:09.687+10:00 | main | ERROR | Besu | Failed to start Besu
picocli.CommandLine$ParameterException: Cannot enable --bonsai-limit-trie-logs-enabled with --sync-mode=FULL and --data-storage-format=BONSAI. You must set --bonsai-limit-trie-logs-enabled=false or use a different sync-mode
```

This also avoids a scenario where private networks can end up starting with sync-mode=FULL and bonsai-limit-trie-logs-enabled=true.

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
        Created At 2024-07-22 03:42:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7356" class=".btn">#7356</a>
            </td>
            <td>
                <b>
                    7288: include WithdrawalRequestPredeployAddress in genesis configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Allow configuration of WithdrawalRequestPredeployAddress in genesis configuration

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
https://github.com/hyperledger/besu/issues/7288

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-22 00:18:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7353" class=".btn">#7353</a>
            </td>
            <td>
                <b>
                    7732: Remove datagas related stuff in favour of blobgas
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Remove datagas related stuff in favour of blobgas
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-19 03:12:39 +0000 UTC
    </div>
</div>

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
                    Fix NPE for legacy ForkId with no forks
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

