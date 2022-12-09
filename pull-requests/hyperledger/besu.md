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
                PR <a href="https://github.com/hyperledger/besu/pull/4798" class=".btn">#4798</a>
            </td>
            <td>
                <b>
                    Runner test refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">dev experience</span><span class="chip">mainnet</span>
            </td>
            <td>
                Refactor to make it easier to find the cause when this tests fails. 
* Deduplicated code. 
* Added a call to peerCount to expose peering issues vs syncing issues
* Because of the async wait() you don't get the exact line where the assertion fails. Added comments for common spots where it fails to make this easier. 
* Also 2 minutes is plenty. 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 01:36:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4797" class=".btn">#4797</a>
            </td>
            <td>
                <b>
                    gradle modifications to support java 19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: lukelee-sl <luke.lee@swirldslabs.com>

Updates to gradle to support java 19.
 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 00:34:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4795" class=".btn">#4795</a>
            </td>
            <td>
                <b>
                    flat database refactor poc 
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
        Created At 2022-12-08 13:39:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4792" class=".btn">#4792</a>
            </td>
            <td>
                <b>
                    Allow starting PoS networks since genesis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description
This PR uses the _vanilla_ `o.h.b.c.MergeBesuControllerBuilder` when the Total Terminal Difficulty is set to **zero** in the genesis.
The main change is in the HEAD commit (25a870a665b429365281dca244723023d0e7fa03), but for making it readable I had to refactor how the `o.h.b.c.BesuControllerBuilder` was constructed, that's in the previous commit (4369a1c3d48f419d5476ad0cfefc24f488f6d0c6). During these changes, I decided to keep an ignored parameter for not adding complexity to the reviewing process.

Note: Judging by the comment in [`o.h.b.c.BesuController:216`](https://github.com/hyperledger/besu/blob/22.10.2/besu/src/main/java/org/hyperledger/besu/controller/BesuController.java#L216) it sounds to me that there is a more comprehensive change waiting to be done, but I'm not familiar enough with the merge architecture to implement it in that way yet and maybe this one is good enough for now.

## Fixed Issue(s)
Fixes #4740 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 07:56:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4791" class=".btn">#4791</a>
            </td>
            <td>
                <b>
                    Docker release builds to no longer add latest tag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Frame <jason.frame@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Changes the docker upload and docker manifest so the latest tag is no longer added for releases. This is necessary so that a release can be built and tested for a period without affecting the docker registry's latest version.

After this PR an additional step will be added as part of the release process after the burn-in period to update the latest tag to the release build.

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
        Created At 2022-12-08 05:53:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4790" class=".btn">#4790</a>
            </td>
            <td>
                <b>
                    Set default curve in EVMTool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Set the curve to the default in the EVM tool durring startup.

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
        Created At 2022-12-08 05:06:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4786" class=".btn">#4786</a>
            </td>
            <td>
                <b>
                    Bugfix snapshot transaction segfaults after storage truncation
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

This PR addresses a race where snap and checkpoint syncs can cause a segfault when starting a worldstate download.  The segfault occurs when rocksdb snapshot transactions are read/written after a storage truncation.  To prevent this and to ensure future uses of clear() and clearFlatDatabase() cannot cause segfaults, this PR:

* adds BonsaiStorageSubscriber type to handle storage events
* moves the subscription model from BonsaiSnapshotWorldStateKeyValueStorage up into BonsaiWorldStateKeyValueStorage
* removes addCachedLayer from TrieLogManager, moves to AbstractTrieLogManager
* TrieLogManager takes a snapshot immediately in addCachedLayer rather than deferring it 
* notifies subscribers on events that can affect the worldstate, specifically:
  * clear (truncate)
  * clearFlatDatabase (truncating a subset of storage)
  * close (closing the worldstate storage

Additionally, only drop cached layers when the worldstate archive has more than the configured number of retained layers.



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
addresses #4765 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 21:26:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4782" class=".btn">#4782</a>
            </td>
            <td>
                <b>
                    Moved besu docs devs to emeritus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Moving two besu docs developers from the besu maintaners group to emeritus status.
@bgravenorst and @NicolasMassart 

Now that the besu-docs have moved to separate repo, this access can be separated. 
The docs repo uses some of the same groups https://github.com/hyperledger/besu-docs/settings/access
but the maintainers one is different https://github.com/orgs/hyperledger/teams/besu-docs-maintainers/members

For besu repos, `triage` is fine. Besu docs developers have to be able to update PRs like adding labels or updating description so that the doc work is easier when the code PR is not detailed enough. 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 21:35:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4781" class=".btn">#4781</a>
            </td>
            <td>
                <b>
                    EIP-4750 EOF Functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

WIP - do not commit

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
        Created At 2022-12-05 20:41:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4780" class=".btn">#4780</a>
            </td>
            <td>
                <b>
                    Speedup modexp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Speed up the gas calculation and execution of the modexp precompile.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 18:37:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4778" class=".btn">#4778</a>
            </td>
            <td>
                <b>
                    Add support for another Transaction Encoder/Decoder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Transaction Encoder/Decoder automatically implied RLP encoding. The 4844 Blob Transaction should be encoded with SSZ encoding.

This PR is a suggestion how to refactor the Encoder to support multiple different types of encodings.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 16:19:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4775" class=".btn">#4775</a>
            </td>
            <td>
                <b>
                    Changed chain download error log level from error to debug.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">logging</span>
            </td>
            <td>
                Signed-off-by: mark-terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Change the log level for a common chain download error from `error` to `debug`.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #4081 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-04 15:20:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4773" class=".btn">#4773</a>
            </td>
            <td>
                <b>
                    Prepare for version 22.10.3-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 22.10.3-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-03 15:44:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4772" class=".btn">#4772</a>
            </td>
            <td>
                <b>
                    Release 22.10.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.10.2
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-03 15:21:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4771" class=".btn">#4771</a>
            </td>
            <td>
                <b>
                    subscribe prior to getting stateTrieNode in cacheStorageNodes
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
ensure storage caching subscribes before accessing worldstate at all

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4765 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 23:35:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4769" class=".btn">#4769</a>
            </td>
            <td>
                <b>
                    prep changelog for 22.10.2
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
add changelog description for 22.10.2 hotfix

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
        Created At 2022-12-02 22:13:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4767" class=".btn">#4767</a>
            </td>
            <td>
                <b>
                    Ensure that Snashot worldstates remain open for async operations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
in 22.10.1, two new operations pre-load account and storage from their respective worldstate asynchronously.  If the worldstate is based on a snapshot, there is a race where the snapshot might be closed ahead of the async operations completing, and subsequently result in a segfault when trying to access a closed rocksdb snapshot.  

This PR adds a subscriber implementation for BonsaiWorldStateKeyValueStorage which ensures that the storage will not be closed while subscribers are still operating on it.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4765 
## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 16:14:17 +0000 UTC
    </div>
</div>

