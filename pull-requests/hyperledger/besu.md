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
                PR <a href="https://github.com/hyperledger/besu/pull/6078" class=".btn">#6078</a>
            </td>
            <td>
                <b>
                    ETC 'Spiral' network upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR adds support to [ECIP-1109](https://ecips.ethereumclassic.org/ECIPs/ecip-1109).
Block number is set to https://github.com/ethereumclassic/ECIPs/pull/514, already set in core-geth in https://github.com/etclabscore/core-geth/pull/571
I also set the DNS discovery tree to what's in [core-geth#bootnodes_mordor.go](https://github.com/etclabscore/core-geth/blob/v1.12.14/params/bootnodes_mordor.go#L29)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 18:48:52 +0000 UTC
    </div>
</div>

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
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span>
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



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-20 14:29:27 +0000 UTC
    </div>
</div>

