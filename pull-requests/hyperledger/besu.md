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
                PR <a href="https://github.com/hyperledger/besu/pull/4812" class=".btn">#4812</a>
            </td>
            <td>
                <b>
                    Memoize transaction size and hash at the same time
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Since to calculate the transaction hash and size, the transaction needs to be encoded to bytes, we can cache both values at the same time, in order to avoid extra expensive encoding tasks.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

relates to  #4724

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-13 18:23:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4811" class=".btn">#4811</a>
            </td>
            <td>
                <b>
                    Possible npe fix
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
This fix was part of PR #4735. I'm separating it because it was not related to the PR itself but was found during some of the tests.

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
        Created At 2022-12-13 06:06:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4810" class=".btn">#4810</a>
            </td>
            <td>
                <b>
                    Docker release task for latest tags
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
Expands the github release workflow to support adding the latest tags for all the docker variants and architectures.

* Replace the use of git sha tags with existing release tags to avoid creating a lot of unneeded tags. When creating the latest tags for all the variants, arch and manifests 15 tags are needed in total
* Added latest tags for variants as was done for previous releases
* Added latest tags for all the architectures
* Added latest tags for multi-arch images

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
        Created At 2022-12-13 01:33:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4807" class=".btn">#4807</a>
            </td>
            <td>
                <b>
                    Non blocking RPC endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This PR converts the standard RPC endpoint in a non blocking one.

## Fixed Issue(s)

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 17:12:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4805" class=".btn">#4805</a>
            </td>
            <td>
                <b>
                    EIP-5450 - EOF Stack Validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

EOF stack validation and omnibus validation changes

Builds off of work for EIP-4200 (#4760) and EIP-4750 (#4781) in addition to already committed "small-EOF" changes EOF-3540 + 3670 (#4644).  Changes to the above PRs will be merged in as updates are committed.

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
        Created At 2022-12-12 15:53:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4804" class=".btn">#4804</a>
            </td>
            <td>
                <b>
                    Fix typo in verkle trie comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: kevaundray <kevtheappdev@gmail.com>

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
        Created At 2022-12-11 18:51:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4803" class=".btn">#4803</a>
            </td>
            <td>
                <b>
                    Fix typo on EthCallTest methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@gmail.com>

## PR description
Fix typos

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-11 11:03:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4802" class=".btn">#4802</a>
            </td>
            <td>
                <b>
                    Add accessList field to Transaction Call Object
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@gmail.com>

## PR description

Besu does not seem to accept AccessList as a parameter:
https://geth.ethereum.org/docs/rpc/objects#transaction-call-object
https://besu.hyperledger.org/en/stable/public-networks/reference/api/objects/#transaction-call-object

## Fixed Issue(s)
#4801

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-11 10:54:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4800" class=".btn">#4800</a>
            </td>
            <td>
                <b>
                    Prepare for version 22.10.4-SNAPSHOT
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
Update version for 22.10.4-SNAPSHOT

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
        Created At 2022-12-09 21:54:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4799" class=".btn">#4799</a>
            </td>
            <td>
                <b>
                    Release 22.10.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.10.3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 21:14:29 +0000 UTC
    </div>
</div>

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
                    Allow starting PoS networks from genesis
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
The main change is in the HEAD commit (25a870a665b429365281dca244723023d0e7fa03), but for making it readable I had to refactor how the `o.h.b.c.BesuControllerBuilder` was constructed, that's in the previous commit (4369a1c3d48f419d5476ad0cfefc24f488f6d0c6). During these changes, I decided to keep an ignored parameter for not adding complexity to the reviewing process, b/c otherwise I would have to change a lot of tests.

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

