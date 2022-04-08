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

This has been split into the following commits:
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
This is a draft b/c it's still missing some items from the _acceptance criteria_

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3686" class=".btn">#3686</a>
            </td>
            <td>
                <b>
                    snapshot version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 18:09:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3685" class=".btn">#3685</a>
            </td>
            <td>
                <b>
                    added issue 3646 to changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 17:01:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3684" class=".btn">#3684</a>
            </td>
            <td>
                <b>
                    Update storage for snapsync and fastsync
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

Modification of the behavior of bonsai storage  in order to avoid deleting everything between two pivot blocks.
The flat database will be deleted between two pivot blocks. And the trie will be used when data is not available in the flat database. During the next writing of this data it will be put automatically in the flat for a faster reading.

This will cause a reduction of the size of the database. Because we will not have data never called in the flat database.

But this may reduce the reading speed when accessing data for the first time. 

For now it will be only activated for snapsync. To check if it's working well  

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
        Created At 2022-04-04 14:20:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3679" class=".btn">#3679</a>
            </td>
            <td>
                <b>
                    [MINOR] update link to P2P spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Previous link to spec is outdated and points to this one 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 06:11:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3678" class=".btn">#3678</a>
            </td>
            <td>
                <b>
                    Don't persist world state when validating block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Frame <jasonwframe@gmail.com>

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
        Created At 2022-04-04 02:32:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3675" class=".btn">#3675</a>
            </td>
            <td>
                <b>
                    Upgrade OpenTelemetry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Upgrades OpenTelemetry to the latest version, and make sure we configure the SDK with environment variables.

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-03 06:51:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3674" class=".btn">#3674</a>
            </td>
            <td>
                <b>
                    Remove Gas object and replace with primitive long
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove the Gas object from the EVM and replace it with the primitive
long. This will have positive impact on short lived object garbage
collection stats, which at very high load causes significant performance
issues.

This also codifies EIP-4803 in the Besu EVM, limiting gas to a signed
64-bit long internally.

There was one notable issue with this transition. Some reference tests
push the limits of memory expansion which results in gas costs over the
EIP limit. The solution is to "clamp" such addition and multiplication
operations at the max or min long value, resulting in the out-of-gas
check failing (such operations will never have a valid execution with
max gas remaining).

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

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
        Created At 2022-04-01 14:07:26 +0000 UTC
    </div>
</div>

