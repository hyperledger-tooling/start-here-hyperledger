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
                PR <a href="https://github.com/hyperledger/besu/pull/3720" class=".btn">#3720</a>
            </td>
            <td>
                <b>
                    revert to TransactionDB to resolve 'busy' exception 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Revert to TransactionDB to resolve 'busy' exception from OptimisticTransactionDB.  

As I understand it, we originally went to OptimisticTransctionDB in order to support `deleteRange()` for our implementation of `RocksDBColumnarKeyBValueStore.clear()`.  In light of the change to the `clear` implementation in #3634, we do not need to use OptimisticTransactionDB.  

Currently in Draft while testing and while discussing the merits of sticking with OptimisticTransactionDB for locking performance.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3719

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 16:48:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3718" class=".btn">#3718</a>
            </td>
            <td>
                <b>
                    [DO NOT MERGE] Test another implementation of Arrays.fill
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Performance test : Test another implementation of Arrays.fill
Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 12:47:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3712" class=".btn">#3712</a>
            </td>
            <td>
                <b>
                    Fix save worldstate issue on bonsai and fastsync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Fix a bug that caused the worldstate to be missing during a fastsync and prevented it from completing properly

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 11:06:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3711" class=".btn">#3711</a>
            </td>
            <td>
                <b>
                    Fix NPE in DeFramer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Catch an NPE using optionals and complete the future nicely with an exception

## Fixed Issue(s)
Fixes #3637 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-08 04:45:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3710" class=".btn">#3710</a>
            </td>
            <td>
                <b>
                    add snapsync as beta feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR enables the snapsync as client. It works with Bonsai but there are still some limitations and possible optimizations.
I will test with Forest

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 09:28:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3709" class=".btn">#3709</a>
            </td>
            <td>
                <b>
                    lgtm yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Added config file for LGTM
Note the LGTM failure is the "main build" which is building off main branch - which still has OOM. But the "merge build" ie building off this PR, is passing. 

Current report: https://lgtm.com/projects/g/hyperledger/besu/logs/rev/pr-935719d01d715dea5db84d624ce75b5505b7708f/lang:java/stage:Build%20main_fe673431fab8c6439e6eb0e83f6545a1583afaeb

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 08:44:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3708" class=".btn">#3708</a>
            </td>
            <td>
                <b>
                    Not null annotations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                replace jetbrains with javax.annotation.Nonnull

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 07:01:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3707" class=".btn">#3707</a>
            </td>
            <td>
                <b>
                    Feature/bonsai fast sync clear flat db
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
During fast sync on bonsai, clear only the flat database rather than the entire bonsai worldstate.  

DRAFT: while testing bonsai fast-sync account db clearing and lazy reads on goerli and mainnet


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Along with #3684 , fixes #3694 

## Documentation


- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 05:19:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3705" class=".btn">#3705</a>
            </td>
            <td>
                <b>
                    vertx 4.2.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Update vertx dependency

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 01:59:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3703" class=".btn">#3703</a>
            </td>
            <td>
                <b>
                    Add flag for snapsync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">snapsync</span>
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

We start adding the flags for the snapsync. Most are experimental flags because normally the user doesn't have to change the values. But it can be used to change the values if needed or to tune performance.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 14:32:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3701" class=".btn">#3701</a>
            </td>
            <td>
                <b>
                    Quorum ATs nightly CI task: setup docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Add docker setup step

Job is currently failing with this error:
docker: Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running?.

eg https://app.circleci.com/pipelines/github/hyperledger/besu/14269/workflows/87252694-72a0-4c5e-845d-0c5be9d09848/jobs/81171

The last time this job passed https://app.circleci.com/pipelines/github/hyperledger/besu/13644/workflows/0fb32713-e855-4cec-b079-680b67f14aa8/jobs/76357

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 06:51:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3699" class=".btn">#3699</a>
            </td>
            <td>
                <b>
                    Enforce trailing peer limits when select pivot block fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Rather than waiting 5 seconds and hoping everything goes well the next run we should run the trailing peer limiter task and drop the useless peers.
## Fixed Issue(s)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 05:29:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3697" class=".btn">#3697</a>
            </td>
            <td>
                <b>
                    Onchain Node Permissioning: log enode being checked with IllegalStateException
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Instead of throwing, log IllegalStateException and the enode that was being checked. and return notPermitted

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 04:31:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3696" class=".btn">#3696</a>
            </td>
            <td>
                <b>
                    Merge: Backward sync re-org below TTD fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Address a post-merge case where we have transitioned to the post-merge rules, but need to import pre-merge blocks due to a reorg ahead of finalization.

BackwardSync is the only mechanism that should be able to reorg below TTD post merge, this PR creates a method In TransitionProtocolSchedule to get ProtocolSpec by block rather than by number.  

TransitionBackwardSyncContext is a transition specific subclass of BackwardSyncContext that leverages the protocol spec by block (without dragging merge consensus into the core ethereum subproject where BackwardSync lives). This backward sync subclass can be removed post-merge with the rest of the transition-by-difficulty code removal.

CURRENTLY DRAFT while writing test coverage.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3688 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 03:55:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3695" class=".btn">#3695</a>
            </td>
            <td>
                <b>
                    Add IPC transport for JSON-RPC APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
Adds socket interface for JSON-RPC, only supported on BSD (OSX) and Linux. This feature has been developed with the intention to reuse and unify, as much as possible, the behaviour among the other transport layers (i.e. HTTP and WS)

Given this is a big PR to review, I have split it in the following commits (I recommend checking them individually):
- [HEAD~7](https://github.com/diega/besu/commit/jsonrpc_ipc~7): Fixes two tests for the HTTP implementation (more info in the commit message)
- [HEAD~6](https://github.com/diega/besu/commit/jsonrpc_ipc~6): Extracts HTTP authentication to its own handler
- [HEAD~5](https://github.com/diega/besu/commit/jsonrpc_ipc~5): Moves authentication handler first in the pipeline, to fail fast **(*)**
- [HEAD~4](https://github.com/diega/besu/commit/jsonrpc_ipc~4): Replaces _timeout handler_ in GraphQL service to use the one provided by Vert.x **(*)**
- [HEAD~3](https://github.com/diega/besu/commit/jsonrpc_ipc~3): Extracts HTTP json parse to its own handler
- [HEAD~2](https://github.com/diega/besu/commit/jsonrpc_ipc~2): Extracts json-rpc execution logic outside of the HTTP handler
- [HEAD~1](https://github.com/diega/besu/commit/jsonrpc_ipc~1): Refactor WS service to use the same execution logic as the HTTP service **(*)**
- [HEAD](https://github.com/diega/besu/commit/jsonrpc_ipc): Implements IPC transport layer

(*): these commits can be omitted without affecting the implementation of the IPC transport

## Note
This implementation has been tested against `geth attach` and it works fine. I also tested Web3J, which works well from an standalone project, but due some strange behaviour in vert.x (ref: [vert.x#4330](https://github.com/eclipse-vertx/vert.x/issues/4330)), I cannot add a test for that into this PR

## Fixed Issue(s)
fixes #535

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 22:15:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3692" class=".btn">#3692</a>
            </td>
            <td>
                <b>
                    Add group heading to command options 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
fixes #2757

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 14:53:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3690" class=".btn">#3690</a>
            </td>
            <td>
                <b>
                    Fix precompile deprecation warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Migrate all the precompiles to the non-deprecated method, making sonar
analysis happy.

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 02:53:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3687" class=".btn">#3687</a>
            </td>
            <td>
                <b>
                    Prep for 22.4.0-RC2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

* Add download links
* update version number
* update changelog
  * one critical change was missed (was not included in original pr)
  * add note about Java 17 migration.



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 19:40:52 +0000 UTC
    </div>
</div>

