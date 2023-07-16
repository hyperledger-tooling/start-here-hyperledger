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
                PR <a href="https://github.com/hyperledger/besu/pull/5708" class=".btn">#5708</a>
            </td>
            <td>
                <b>
                    replace ArrayList with HashSet for rpcMethodExists check
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
When executing the RpcMethod.rpcMethodExists(String rpcMethod) method, using HashSet instead of ArrayList provides a very very small performance improvement of a few nanoseconds. 😂😂


## Fixed Issue(s)
nothing
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-16 09:09:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5706" class=".btn">#5706</a>
            </td>
            <td>
                <b>
                    Append ABI-decoded revert reason to message field in error responses
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Currently in draft. Todo:

- [ ] Unit tests
- [ ] Changelog
- [ ] Docs update

This PR does the following:

- Adds a helper function to `JsonRpcErrorResponse` to decode revert reasons
- Adds a private member variable `reason` to `JsonRpcError` which can optionally be set
- Appends the `reason` to the response from `JsonRpcError.getMessage()` so that whenever the message for a JSON RPC error is retrieved, any reason that is set is included e.g. `Execution reverted: ERC20: transfer amount exceeds balance`

__Note__: this is proposed as a change to existing behaviour. It is assumed (rightly or wrongly) that existing applications will most likely use `startsWith("Execution reverted")` or other language equivalent, to parse error responses today. The fact that Quorum returns errors in this format (and that there isn't an option to exclude the decoded reason) suggests that any application not using `startsWith` semantics for error parsing is already brittle to different ethereum clients. It could be made configurable in Besu (perhaps with a `--exclude-decoded-reason` or similar option) but my personal view is to treat this as a fix to existing behaviour and document it in the changelog accordingly. I'm open to other opinions on this from reviewers.

Example error response before this PR:

```
{
    "jsonrpc": "2.0",
    "id": 1,
    "error": {
        "code": -32000,
        "message": "Execution reverted",
        "data": "0x08c379a00000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000002645524332303a207472616e7366657220616d6f756e7420657863656564732062616c616e63650000000000000000000000000000000000000000000000000000"
    }
}
```

Example error response with this PR:

```
{
    "jsonrpc": "2.0",
    "id": 1,
    "error": {
        "code": -32000,
        "message": "Execution reverted: ERC20: transfer amount exceeds balance",
        "data": "0x08c379a00000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000002645524332303a207472616e7366657220616d6f756e7420657863656564732062616c616e63650000000000000000000000000000000000000000000000000000"
    }
}
```

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/5705
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 09:19:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5704" class=".btn">#5704</a>
            </td>
            <td>
                <b>
                    switch RlpBlockImporter tests to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## Migrate RlpBlockImporterTest from JUnit 4.0 to JUnit 5.0 #5571

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
#5571 
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 06:47:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5703" class=".btn">#5703</a>
            </td>
            <td>
                <b>
                    Plugins migrate to junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                Migrate the plugins module from JUnit 4.0 to JUnit 5.0
fixes https://github.com/hyperledger/besu/issues/5559

Builds off commits in #5582 from @7suyash7  - thanks for you contribution!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 01:34:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5702" class=".btn">#5702</a>
            </td>
            <td>
                <b>
                    EIP-4844 testing support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Add two new fields to reference tests (versionedHashes, maxFeePerDataGas) 
* Rename DataHash to BlobHash (to align with EIP4844 text)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-13 23:44:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5701" class=".btn">#5701</a>
            </td>
            <td>
                <b>
                    Changes to allow evmtool t8n-server to work with execution-spec-tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                An omnibus of minor changes needed for t8n-server to work with the EFs new execution-spec-tests framework

* Reduce logging output
* Fix json library mismatch between t8n and t8n-server
* Add hook to enumerate supported forks
* temporarily map Shanghai+6780 to Cancun
* add to main distro under 'evmtool' name

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-13 15:37:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5700" class=".btn">#5700</a>
            </td>
            <td>
                <b>
                    Promote segmented storage
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
DRAFT STATUS - WIP

At a high level, this PR promotes SegmentedKeyValueStorage into the plugin-api for storage.  

The primary benefit of this besides addressing tech debt is that we can directly use segmented storage and atomically commit across multiple segments.  This is mainly beneficial for bonsai worldstate, which comprises four separate key value store segments.  

This is motivated by "unclean" worldstate storage that can result from besu app or the host machine crashing for a variety of reasons.  RocksDB handles unclean shutdowns very well, but if the besu application was in the midst of a worldstate commit, each of the individual worldstate storages might be in different states of commit/rollback at the time of the crash.  By having composed storage, we can rely on the guarantees of rocksdb to atomically commit or rollback changes in the event of a crash or halt, like what resulted in #5576 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5362 #5576 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-13 14:02:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5699" class=".btn">#5699</a>
            </td>
            <td>
                <b>
                    update fcu
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

We have identified a potential issue with the FCU mechanism. Based on the logs, it seems that Besu considers each new head as a reorganization (reorg) because of this line https://github.com/hyperledger/besu/blob/main/consensus/merge/src/main/java/org/hyperledger/besu/consensus/merge/blockcreation/MergeCoordinator.java#L610 so we are not updating the worldstate if the new head is not a direct descendant of the current head, which is rare in general. As a result, we enter the "rewindToBlock" method https://github.com/hyperledger/besu/blob/main/consensus/merge/src/main/java/org/hyperledger/besu/consensus/merge/blockcreation/MergeCoordinator.java#L633, which performs a chain reorg (in this case, a move forward of the chain) without changing the world state. However, with Prysm, we only encounter this case and keep advancing the chain without advancing the world state. Consequently, with each "engineNewPayload" call, we need to apply a larger number of trie logs to process the new block, which leads to a node crash.

Upon examining the code, it is indeed not normal to have a scenario where we change the blockchain without changing the world state.

Indeed, the same issue applies to the engineNewPayload operation. If the distance between the head and the payload we want to execute is too large, it is necessary to trigger a backward sync to reach the latest finalized block instead of attempting to roll forward an impossible number of trie log operations. This ensures the stability and proper functioning of the node.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-13 09:17:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5698" class=".btn">#5698</a>
            </td>
            <td>
                <b>
                    remove v0 version of the database
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

This version of the database is not used anymore so we can remove it 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 13:28:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5693" class=".btn">#5693</a>
            </td>
            <td>
                <b>
                    Do not leak references to PendingTransactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamChupa</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR complete the work done in #5634, basically since the latter is creating and modifying the `pendingTransactions` object at runtime, references to that field outside the txpool, must not be allowed anymore, otherwise object that cached a reference to `pendingTransactions` could see an uninitialized or stale object.

With this PR it is not possible anymore to get references directly to the `pendingTransactions` object and all the interaction previously done with it, now go through `TransactionPool` that manages that lifecycle of the `pendingTransactions` object.

Do not be scared by the number of changes in this PR, since the it is mostly about using `TransactionPool` instead of `PendingTransactions` and unit tests adjustments.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fix an issue introduced by #5634 that causes block proposals with 0 transactions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 10:52:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5691" class=".btn">#5691</a>
            </td>
            <td>
                <b>
                    [4844] KZGPointEvalPrecompiled - Use PrecompileContractResult methods to halt and succeed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">4844</span>
            </td>
            <td>
                ## PR description

- Use PrecompileContractResult methods to halt and succeed;
- Do not return Bytes.Empty
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 06:47:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5690" class=".btn">#5690</a>
            </td>
            <td>
                <b>
                    [4844] New Payload V3 - Return Invalid Payload instead of Invalid Params for invalid versionedHash version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">4844</span>
            </td>
            <td>
                ## PR description

- Return an invalid payload instead of an internal error in case of an invalid version hash.
- Fix calculated hashes validation

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 06:38:42 +0000 UTC
    </div>
</div>

