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
                PR <a href="https://github.com/hyperledger/besu/pull/6089" class=".btn">#6089</a>
            </td>
            <td>
                <b>
                    Introduce a timeout for the evaluation of a single tx during block creation
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
        Created At 2023-10-25 15:28:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6088" class=".btn">#6088</a>
            </td>
            <td>
                <b>
                    Fix k8s nat manager logic and add `--Xnat-kube-service-namespace` flag
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
Now the Kubernetes nat manager requires cluster-wide permissions (list service resources in all namespaces). Also, it has a bug: when multiple besu networks are configured in the same cluster with the same service names in different namespaces, the nat manager may set an inappropriate IP address for the besu node due to enumerating services from all namespaces and checking only their names.

I suggest adding a new flag: `--Xnat-kube-service-namespace` to specify a concrete besu node service namespace and not use a list of services, but a get request for a specific service.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5002
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 13:09:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6087" class=".btn">#6087</a>
            </td>
            <td>
                <b>
                    TraceService: return results for transactions in block
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

* The TraceService returns the result of the processed transactions
* In case of an internal error during tx processing, the stack trace is added to the error message as well.

## Fixed Issue(s)
fixes #6077 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 12:44:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6085" class=".btn">#6085</a>
            </td>
            <td>
                <b>
                    create trielog state for tracing
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

fixes #6050 
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 08:53:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6083" class=".btn">#6083</a>
            </td>
            <td>
                <b>
                    Add transaction selector based on min priority fee parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add transaction selector based on min priority fee parameter

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 07:35:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6082" class=".btn">#6082</a>
            </td>
            <td>
                <b>
                    Add option to clique to skip creating empty blocks
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
Add an option to clique to skip creating empty blocks

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 06:50:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6081" class=".btn">#6081</a>
            </td>
            <td>
                <b>
                    Bump 23.10.1-RC to 23.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Bump 23.10.1-RC to 23.10.1 on release branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-25 01:55:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6080" class=".btn">#6080</a>
            </td>
            <td>
                <b>
                    Implement miner_setMinPriorityFee and miner_getMinPriorityFee
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
Built on top of https://github.com/fab-10/besu/tree/min-priority-fee, which adds `--min-priority-fee` CLI option

Adds two new JsonRPC methods: 

- miner_setMinPriorityFee - Sets the value of `miningParameters.minPriorityFeePerGas`
- miner_getMinPriorityFee - Returns the current value of `miningParameters.minPriorityFeePerGas`

This PR does not add the transactionSelector based on `minPriorityFeePerGas`. It will be added in a different PR

Examples: 

Example:  
Request
`{"jsonrpc":"2.0","id":1,"method":"miner_setMinPriorityFee","params":[1]}`
Response:
```
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": true
}
```
Invalid request: 
` {"jsonrpc":"2.0","id":1,"method":"miner_setMinPriorityFee","params":[-1]}
`Response:
```
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": false
}
```
Get method:
` {"jsonrpc":"2.0","id":1,"method":"miner_getMinPriorityFee","params":[]}
`Response:
```
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": 7
}
```




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 22:53:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6079" class=".btn">#6079</a>
            </td>
            <td>
                <b>
                    Force tx replacement price bump to zero when zero base fee market is configured
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

This PR allows to replace txs on zero base fee markets, or on gas price network, where the txs have gas price set to zero (with `min-gas-price=0`).

To achieve that we force the `tx-pool-price-bump=0` when the `zeroBaseFee:true` genesis option is present.
But this was not enough, since the transaction replacement rules were forcing the new price to be strictly greater than the price bump, that in my opinion is not intuitive, since for example if your existing tx has a gas price of 100, and the price bump is 10%, then we should accept a valid replacement a tx with a gas price of 110, and not 111 as it was before.
So the other change is to accept, as valid replacement, tx with a gas price greater than or equal to the price bump. This make also the `tx-pool-price-bump=0` case more intuitive, since you can replace a tx without increasing the gas price.

`doc-change-required` to explain that if `zeroBaseFee:true` in the genesis, then `tx-pool-price-bump=0` is forced internally, and any attempt to specify a value for it results in an error

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #6043
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 19:11:42 +0000 UTC
    </div>
</div>

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
                PR <a href="https://github.com/hyperledger/besu/pull/6075" class=".btn">#6075</a>
            </td>
            <td>
                <b>
                    Continuous Trie Log Pruning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Feature toggled by `--Xtrie-log-pruning-enabled`
- Add trie log pruning after a successful `TrieLogManager.saveTrieLog`
- Each time a trie log is persisted, the current trie log is cached and the pruner is run against the oldest entries in the cache.
- This makes no attempt to manage the backlog of old trie logs, it will only prune what has been added to the cache, i.e. trie logs that have been added since the feature was enabled.
- Pruner limit exists in case of exceptional circumstances, but we should only ever be pruning all the forks for a single block number during each prune execution.

This is a second take of https://github.com/hyperledger/besu/pull/6026
Currently built on https://github.com/hyperledger/besu/pull/6072 (diff: https://github.com/siladu/besu/compare/refactor-trie-log-manager...trie-log-pruning-take2)

One downside of this PR compared to #6026 is that restarting besu may leave a gap in the pruned trie logs because we don't preload the cache. This will have to be considered as part of managing the backlog. It may mean that we can't simply rely on a "one-off" resync or prune subcommand. However, these un-pruneable trie logs should be negligible compared to the saving gained for long running nodes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 06:26:23 +0000 UTC
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
                    Cherry-pick  main into release 23.10.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Cherry-pick main into release 23.10.x

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

