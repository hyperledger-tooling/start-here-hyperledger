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
                PR <a href="https://github.com/hyperledger/besu/pull/6074" class=".btn">#6074</a>
            </td>
            <td>
                <b>
                    Trigger contextEnter/Exit for all frames, including root
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Filtering out the root context from the `context{Enter,Exit}` tracing hook leads to an asymmetry of treatment when returning from a create/call context, where the root context is blind to the event, but non-root contexts can read it.

This PR disables this restriction to address this blindspot.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-23 22:44:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6073" class=".btn">#6073</a>
            </td>
            <td>
                <b>
                    feat: add a way to read memory without altering the word capacity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Objects using the `MessageFrame` may wish to immutably read the memory of the frame without altering the word capacity of the memory, i.e. a “shadow” read as it behaves transparently w.r.t. the EVM.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-23 12:20:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6072" class=".btn">#6072</a>
            </td>
            <td>
                <b>
                    Decouple TrieLogManager and CachedWorldStorageManager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Two concepts were mixed together via inheritance:
1. trie log management
2. caching world states

This PR splits these concepts out ahead of adding in trie log pruning.

CachedWorldStorageManager is added as a field alongside TrieLogManager in BonsaiWorldStateProvider.

Following previous refactors, there's now no need to have an AbstractTrieLogManager or TrieLogManager interface
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-23 03:36:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6071" class=".btn">#6071</a>
            </td>
            <td>
                <b>
                    Optimize GetPooledTransactionsFromPeerTask with HashSet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Overview
This PR optimises `GetPooledTransactionsFromPeerTask` by switching from using a `List<Hash>` to a `HashSet<hash>` for transaction hashes, significantly reducing overhead associated with hash lookups.

### Changes
- Refactor `GetPooledTransactionsFromPeerTask` to use `HashSet` for transaction hashes.
- Made minor logic adjustments to accommodate the data structure change.

### Performance Improvements
Before: 
![Screenshot from 2023-10-22 12-25-52](https://github.com/hyperledger/besu/assets/89125422/46d3dc63-cc2c-4e28-a5fb-1ac5ef6f6d00)

After:
![Screenshot from 2023-10-22 12-46-53](https://github.com/hyperledger/besu/assets/89125422/d8822aa0-3e4f-4f8a-841d-8b5874c4cd65)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-22 09:33:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6069" class=".btn">#6069</a>
            </td>
            <td>
                <b>
                    Use Bytes Trie to track warm addresses
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move from a java HashSet to a custom Trie based on bytes to store the warm addresses, creates, and self-destructs.

This avoids needing to calculate java hashes or engage in using custom Comparators.

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
        Created At 2023-10-20 20:29:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6068" class=".btn">#6068</a>
            </td>
            <td>
                <b>
                    Migrate Operand Stack to Growing Stack Pool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To improve the performance of CALL operations move the OperandStack and ReturnStack to growing stacks instead of a fully allocated stack.

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
        Created At 2023-10-20 18:26:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6067" class=".btn">#6067</a>
            </td>
            <td>
                <b>
                    Don't put NONCE_TOO_LOW transactions into the invalid nonce cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This is intended to improve the issue described in https://github.com/hyperledger/besu/issues/6058. I don't think it fixes every possible case, but from testing it seems to be old transactions from a node, which are now all `NONCE_TOO_LOW`, that can cause this problem.

## Fixed Issue(s)
See https://github.com/hyperledger/besu/issues/6058 - although it may not be completely fixed after this PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-20 16:16:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6066" class=".btn">#6066</a>
            </td>
            <td>
                <b>
                    Update to production KZG ceremony output
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - update to new library
- disable KZG testing on static test vectors till new ones are available


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-20 14:29:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6064" class=".btn">#6064</a>
            </td>
            <td>
                <b>
                    Cherry-pick  main into release 22.10.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Cherry-pick main into release 22.10.x

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-20 01:51:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6062" class=".btn">#6062</a>
            </td>
            <td>
                <b>
                    Update changelog release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix changelog - Add issue numbers
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-20 00:24:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6060" class=".btn">#6060</a>
            </td>
            <td>
                <b>
                    Dencun corner cases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                cherry pick 2 changes from #6054 
* EIP-3541 regression in Cancun - https://github.com/hyperledger/besu/pull/6054/files#diff-22b78733e37a697fa8d1d8a02d2a87fe5ccea9cf67c34ce5e6311f024c14abd6L643-R738
* EIP-4788 conformance corner case - https://github.com/hyperledger/besu/pull/6054/files#diff-61db834b59eae5ce5c438462505de1add8fa244deda830742060d15f668a9806R39-R44
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 23:58:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6059" class=".btn">#6059</a>
            </td>
            <td>
                <b>
                    Trie log blobdb
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
Move trie log storage to blobdb

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See #5866 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 22:59:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6057" class=".btn">#6057</a>
            </td>
            <td>
                <b>
                    Code storage by hash compare
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
This is a fork of https://github.com/hyperledger/besu/pull/5889 to test the accuracy of the code storage.

Not intended to be merged.
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 01:25:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6056" class=".btn">#6056</a>
            </td>
            <td>
                <b>
                    Code storage by hash nodelete
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
This is a fork of #5889 to test the impact of not deleting and removing the code.

Not intended to be merged.
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 00:29:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6054" class=".btn">#6054</a>
            </td>
            <td>
                <b>
                    Update reference tests to Cancun
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update reference tests to cancun tests.

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
        Created At 2023-10-18 22:34:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6052" class=".btn">#6052</a>
            </td>
            <td>
                <b>
                    not pruning block during the initial sync
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

I propose a modification to the block pruning feature so that we can lower the minimum limit to 512 instead of 7200. Why 512? Simply to allow a minimum number of blocks close to the head. This is also the number we chose for the world state on Bonsai and seems to be a good compromise between pruning and accessibility of recent history.

7200 was chosen to avoid pruning during the initial sync, so I made a modification to prune during the initial sync by querying the SyncState.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 13:14:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6049" class=".btn">#6049</a>
            </td>
            <td>
                <b>
                    [MINOR] ux improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * log plugins summary at info (part of config overview)
* include affected CLI option when there's a compatibility issue found by `failIfOptionDoesntMeetRequirement`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 05:27:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6048" class=".btn">#6048</a>
            </td>
            <td>
                <b>
                    Use BONSAI for the execution engine BesuNode in ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Affects tests extending AbstractJsonRpcTest

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 23:05:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6047" class=".btn">#6047</a>
            </td>
            <td>
                <b>
                    Add X (Twitter) to README, Fix Roadmap Hyperlink
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

- Adds X (Twitter) hyperlink to README for increased visibility and community engagement for the Hyperledger Besu account.

- Fixes roadmap hyperlink as previous one is broken.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 22:14:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6046" class=".btn">#6046</a>
            </td>
            <td>
                <b>
                    Unsigned timestamps and blob gas used
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merge after pr #6037 , was built on top of that.

the pyspec simulator in Hive likes to check fields for max capacities, which showed us a lot of places where using signed longs is a problem. This pr fixes many of them.

broader adoption of CheckerFramework is suggested at a later time, so that we can see where else we are affected by this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 18:26:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6045" class=".btn">#6045</a>
            </td>
            <td>
                <b>
                    Fixed eth_call before london fork for the calls without strict parameter
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
Fixed eth_call before London fork for the calls without `strict` parameters.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fix #5943
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 17:31:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6044" class=".btn">#6044</a>
            </td>
            <td>
                <b>
                    Time limited block creation
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
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 17:04:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6040" class=".btn">#6040</a>
            </td>
            <td>
                <b>
                    Fix 23.10.0 Breaking Changes changelog entry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes a wrong breaking change entry reported here #6031

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 07:59:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6038" class=".btn">#6038</a>
            </td>
            <td>
                <b>
                    [CHANGELOG] fix links to issue 5772
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes link refs #6031 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 01:50:51 +0000 UTC
    </div>
</div>

