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
                PR <a href="https://github.com/hyperledger/besu/pull/4261" class=".btn">#4261</a>
            </td>
            <td>
                <b>
                    getProof encoding fix for 4249
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
Addresses encoding issue in eth_getProof, see https://ethereum.github.io/execution-apis/api-documentation/

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4249
## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 17:26:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4260" class=".btn">#4260</a>
            </td>
            <td>
                <b>
                    implement tentative mainnet TTD
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

Draft until after ACD call on 2022-11-18

https://github.com/ethereum/execution-specs/pull/585

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
        Created At 2022-08-15 16:49:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4259" class=".btn">#4259</a>
            </td>
            <td>
                <b>
                    Simplify Trie Dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Make the ethereum/trie and services/kvstore modules  as slim as possible
by dropping dependencies.

* The ':util' api dependency is removed from kvstore  and added to
  downstream modules
* Move tries's kvstore dependency to test
* other dependencies are removed as unused from trie and kvstore


<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 16:11:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4256" class=".btn">#4256</a>
            </td>
            <td>
                <b>
                    Refactor and fix retrying get block switching peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This is built on top of #4254, so if not merge yet, check it before this one.

RetryingGetBlockFromPeersTask had a problem that prevented to complete
when all the peers fail, and that also had the
consequence to not removing the failed requested block from the internal
caches in BlockPropagationManager, that could cause a stall since that
block will to be tried to be retrieved again.

Made also an abstraction of a retrying peer task that tries a different peer on every execution, so it can used also for other tasks

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
        Created At 2022-08-12 16:20:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4255" class=".btn">#4255</a>
            </td>
            <td>
                <b>
                    Feature/rollback with snapshot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
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
        Created At 2022-08-12 12:32:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4254" class=".btn">#4254</a>
            </td>
            <td>
                <b>
                    Fix off-by-one error in AbstractRetryingPeerTask
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Currently tasks based on AbstractRetryingPeerTask, execute the actual task maxRetries + 1 times, while devs expect that it will be executed exactly maxRetries times.

Incremented the maxRetries in existing code to reflect the previous behavior of having the actual number of executions equals to maxRetries + 1.

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
        Created At 2022-08-11 17:50:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4251" class=".btn">#4251</a>
            </td>
            <td>
                <b>
                    Enable dependency verification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This PR enables [dependency verification](https://docs.gradle.org/current/userguide/dependency_verification.html) using a mechanism [introduced in Gradle 6.2](https://docs.gradle.org/6.2/release-notes.html#dependency-verification).

The `gradle/verification-metadata.xml` file was autogenerated relying on the [TOFU](https://en.wikipedia.org/wiki/Trust_on_first_use) scheme.

There are three commits in this PR:
 - `HEAD~2`: adds auto generated sha-256 checksums
 - `HEAD~1`: adds missing sha-256 checksum manually
 - `HEAD`: adds signature verification

Surprisingly, there were some signing keys that had to be ignored b/c they were missing from public repositories. I leave here the list of those unsigned artifacts for future reference:
- discovery-22.2.0.module
- discovery-22.2.0.pom
- quorum-mainnet-launcher-1.0.1.pom
- junit-4.12.jar
- junit-4.12.pom
- bcprov-jdk15on-1.68.jar
- bcprov-jdk15on-1.68.pom
- mxparser-1.2.1.pom
- mxparser-1.2.2.jar
- mxparser-1.2.2.pom
- xstream-1.4.17.pom
- xstream-1.4.19.jar
- xstream-1.4.19.pom
- xstream-parent-1.4.17.pom
- xstream-parent-1.4.19.pom
- kotlinpoet-1.5.0.jar
- kotlinpoet-1.5.0.pom
- build-info-api-2.36.3.jar
- build-info-api-2.36.3.pom
- build-info-client-2.36.3.jar
- build-info-client-2.36.3.pom
- build-info-extractor-2.36.3.jar
- build-info-extractor-2.36.3.pom
- build-info-extractor-gradle-4.28.3.jar
- build-info-extractor-gradle-4.28.3.pom
- file-specs-java-1.1.1.jar
- file-specs-java-1.1.1.module
- dependency-management-plugin-1.0.11.RELEASE.jar
- dependency-management-plugin-1.0.11.RELEASE.pom
- apache-7.pom
- plexus-2.0.7.pom
- plexus-component-annotations-1.5.5.jar
- plexus-component-annotations-1.5.5.pom
- plexus-components-1.1.18.pom
- plexus-containers-1.5.5.pom
- plexus-interpolation-1.14.jar
- plexus-interpolation-1.14.pom
- plexus-utils-2.0.5.pom
- plexus-utils-2.0.6.jar
- plexus-utils-2.0.6.pom

Accepting this PR means that every time a dependency is upgraded, this file needs to be updated too. I think this is a positive thing, since it will make the dev more aware of what the upgrade really implies dependecy wise.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 18:30:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4241" class=".btn">#4241</a>
            </td>
            <td>
                <b>
                    quieten DynamicPivotBlockManager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">logging</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
* Only change pivot block if it is different than the existing syncTarget pivotBlock
* move logging level to debug

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #4211
## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 23:36:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4240" class=".btn">#4240</a>
            </td>
            <td>
                <b>
                    remove MergeUnfinalizedValidationRule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
The CL is allowed to reorg around finalized via social consensus.  Remove this validation rule and rely solely on the CL for that social coordination.

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
        Created At 2022-08-09 18:38:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4237" class=".btn">#4237</a>
            </td>
            <td>
                <b>
                    Better management of jemalloc presence/absence
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">logging</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

If jemalloc is not present, an error message is printed, but the absence of jemalloc is not a real error, so in this PR we try to understand if jemalloc is available and print messages that are easier for the user to understand, and invite him to install jemalloc to get better memory usage

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
        Created At 2022-08-09 13:59:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4236" class=".btn">#4236</a>
            </td>
            <td>
                <b>
                    Always switch full sync target when local chain is close to chain head
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Full sync has a sync target stability feature that works well when syncing from genesis, but is not optimal when the initial sync is done and local chian head is equal or very close to the target head, when the stability feature could prevent switching to the best peer.

By default the stability feature prevent to switch to the best peer, if its height is not 200 block greather, or the difficulty is not 1_000_000_000_000_000_000L greather than the current sync target. 

These value are too large when we are already in sync and just need to follow the best peer, so this PR, changes only enable the stability feature when the current chain head is far from the target head, that occurs when doing a full sync from genesis or when you restart Besu after some hours or days.

This can help Besu to stay in sync, because if the block propagation manager is missing some blocks, then it stops caching incoming blocks when the distance with the local chain head is > 30, but since the chain state of a peer is only updated when a new block is seen from that peer, there could not be enough information for the current sync target switching strategy to switch to the best peer.

On an already synced node, there are 2 hidden configuration flags to always for the switch to the best peer, without this patch:
`--Xsynchronizer-downloader-change-target-threshold-by-td=0`
`--Xsynchronizer-downloader-change-target-threshold-by-height=0`


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

potential fix for #3955

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 12:20:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4234" class=".btn">#4234</a>
            </td>
            <td>
                <b>
                    peer count - just count the live ones
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

This does not address the root cause, but will address the problem of users complaining that the logs report too many peers.

This should mean that the number of peers reported in the logs will be the correct number ie the number of connected peers

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 10:18:45 +0000 UTC
    </div>
</div>

