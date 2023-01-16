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
                PR <a href="https://github.com/hyperledger/besu/pull/4912" class=".btn">#4912</a>
            </td>
            <td>
                <b>
                    Increase cache performance post snapshot fix
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

We detected a regression in the cache after the fix of the snapshot segfault issue. This is due to the fact that the cache tried to use a worldstate storage that was unavailable too soon (not subscribe because shouldClose is true). The cache did not have time to preload enough node and so the calculate root hash is less efficient

the issue is 

- In the validateAndProcessBlock we are doing a copy of the worldState
```java
      try (final var worldState =
        context
            .getWorldStateArchive()
            .getMutable(parentHeader.getStateRoot(), parentHeader.getBlockHash(), shouldPersist)
            .map(
                ws -> {
                  if (!ws.isPersistable()) {
                    return ws.copy();
                  }
                  return ws;
                })
            .orElse(null)) {
```

In our case it was BonsaiLayeredWorldstate

```java
public MutableWorldState copy() {
    // return an in-memory worldstate that is based on a persisted snapshot for this blockhash.
    try (SnapshotMutableWorldState snapshot =
        archive
            .getMutableSnapshot(this.blockHash())
            .map(SnapshotMutableWorldState.class::cast)
            .orElseThrow(
                () ->
                    new StorageException(
                        "Unable to copy Layered Worldstate for " + blockHash().toHexString()))) {
      return new BonsaiInMemoryWorldState(archive, snapshot.getWorldStateStorage());
    } catch (Exception ex) {
      throw new RuntimeException(ex);
    }
  }
```

In this code we can see that we are getting a snapshot and passing the worldstate storage of this snapshot to the BonsaiInMemoryWorldState class. It is a try -with-resources statement so the snapshot will be close at the end of the copy

The close of the snapshot will call the close method of the worldstate storage but this one will not be close because BonsaiInMemoryWorldState subscribed to it . The close snapshot will not close the storage but will set the shouldClose to true. And this is the problem.

when the cache try to subscribe to worldstate storage an exception is raised because this shouldClose is true even if the worldstate is still open 

```java
public synchronized long subscribe(final BonsaiStorageSubscriber sub) {
    if (shouldClose.get()) {
      throw new RuntimeException("Storage is marked to close or has already closed");
    }
    return super.subscribe(sub);
  }
```

The idea is to use isClosed instead of shouldClose during the subscribe 

Here come CPU profiling flame graphs that show the difference before and after the regression 
**Before**

- Calculate Root Hash (Pink part)

<img width="1718" alt="image" src="https://user-images.githubusercontent.com/5099602/212098966-c6b11e66-9e1d-4b4c-a8a9-e9772a9a4746.png">

- Cache Preload

<img width="1718" alt="image" src="https://user-images.githubusercontent.com/5099602/212096887-9a97ae9e-026e-46c9-a9c3-e0040786bd0e.png">

**After**

- Calculate Root Hash (Pink part)

<img width="1718" alt="image" src="https://user-images.githubusercontent.com/5099602/212100089-93f9a402-f3e0-407c-9369-8770dd53ff9b.png">

- Cache Preload
![image](https://user-images.githubusercontent.com/5099602/212104122-77e42da9-2e3c-40b8-a8fb-87ddc326ae84.png)

Zoom on the code snippet that triggers the runtime exception
<img width="1718" alt="image" src="https://user-images.githubusercontent.com/5099602/212097985-f4e5a740-dfc9-495a-953a-77a75794daa4.png">


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
        Created At 2023-01-12 14:36:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4911" class=".btn">#4911</a>
            </td>
            <td>
                <b>
                    EIP-3860 Initcode Size Reference Test fixes
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

Fix corner cases around initcode size checking in reference tests.

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
        Created At 2023-01-12 04:13:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4909" class=".btn">#4909</a>
            </td>
            <td>
                <b>
                    Add engine get payload body
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Zhenyang Shi <wcgcyx@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR adds two new engine APIs: engine_getPayloadBodiesByHashV1 and engine_getPayloadBodiesByRangeV1.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4787 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-12 01:21:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4908" class=".btn">#4908</a>
            </td>
            <td>
                <b>
                    Prepare for version 23.1.0-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 23.1.0-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-12 00:25:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4907" class=".btn">#4907</a>
            </td>
            <td>
                <b>
                    Release 23.1.0-RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.1.0-RC1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 23:56:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4906" class=".btn">#4906</a>
            </td>
            <td>
                <b>
                    Address bonsai self-destruct stale code present 
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
During an initial worldstate sync, a self-destruct that occurs between the initial pivot block and final heal pivot block will leave stale code in bonsai code storage.  If subsequently the code is redeployed via create2 to the same contract address, the bonsai db will fail to roll code changes to the block where the redeployment occurs.  This presents in a handful of ways such as 'worldstate not present' or 'unable to copy layered worldstate'.

Discussing with @matkt, since the repivot and heal process does not presently have an opportunity to 'heal' the code storage, and we should be able to trust the trielogs, this PR changes the rollCodeForward behavior to overwrite stale code if/when it is found.  This should resolve #4784 and give the besu team an opportunity to revisit this in flat database heal work that is ongoing.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
addresses #4784 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 16:05:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4905" class=".btn">#4905</a>
            </td>
            <td>
                <b>
                    Ibft1 deprecation warning
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
Add IBFT1 deprecation warning.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fix #4851
related to #4839

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 03:02:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4902" class=".btn">#4902</a>
            </td>
            <td>
                <b>
                    [RPC] add SAFE and FINALIZED options for block param
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">RPC</span>
            </td>
            <td>
                RPC method changes
- add SAFE and FINALIZED options for block param
- check length of blockNumber / blockHash param - if it's too short to be a blockHash and too long to be a blockNumber, throw Invalid params
- added some extra tests. Specifically this file `eth_getTransactionCount_invalidBlockNumber.json` - without the code changes in this PR, that spec test returns "block not found", with these changes returns Invalid params

See #4233 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 05:02:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4900" class=".btn">#4900</a>
            </td>
            <td>
                <b>
                    Support Shanghai in Reference Tests
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

Add support for Shanghai in reference tests
* Add Shanghai and Cancun milestones
* Add "withdrawals" and "withdrawalsRoot" to json objects
* Migrate to schedule by block header.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

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
        Created At 2023-01-09 23:07:41 +0000 UTC
    </div>
</div>

