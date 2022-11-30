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
                PR <a href="https://github.com/hyperledger/besu/pull/4753" class=".btn">#4753</a>
            </td>
            <td>
                <b>
                    Print the debug rpc params as serialized json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">logging</span><span class="chip">RPC</span>
            </td>
            <td>
                 This makes it easier to copy-paste requests when debugging...
 
 e.g.

Before:
```
JSON-RPC request -> engine_forkchoiceUpdatedV1 [{headBlockHash=0x837000f0dde4caf071e7e6d9e27da4160b8c2ee26e20942a971b5628ddb3d98a, safeBlockHash=0x0000000000000000000000000000000000000000000000000000000000000000, finalizedBlockHash=0x0000000000000000000000000000000000000000000000000000000000000000}, {timestamp=0x6386e3d6, prevRandao=0xe60e73f998d2b7a33844255506c80b9d5fb8065792152a0dff9a59293b9e556e, suggestedFeeRecipient=0xa94f5374fce5edbc8e2a8697c15331677e6ebf0b}]
```

After:
```
JSON-RPC request -> engine_forkchoiceUpdatedV1 [{"headBlockHash":"0x3e04c0c8b14a325ef0946afb76bd3cd0a2e8670c945cf1b17d77d8f2ff6f7aaa","safeBlockHash":"0x0000000000000000000000000000000000000000000000000000000000000000","finalizedBlockHash":"0x0000000000000000000000000000000000000000000000000000000000000000"},{"timestamp":"0x6386e2e4","prevRandao":"0x44321cbd5b10ab399c772dc3f716702b9c82f79fcb8014eb9bb3afd3fbd59edb","suggestedFeeRecipient":"0xa94f5374fce5edbc8e2a8697c15331677e6ebf0b"}]
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 04:44:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4752" class=".btn">#4752</a>
            </td>
            <td>
                <b>
                    Hidden option  to enforce an eth capability maximum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Create a hidden flag to force an eth capability maximum. With future versions of the protocol being implemented, we may need an easy way to compare capabilities without having to change the code every time. 
 
This PR implements the flag `--Xeth-max-capability-enabled` to enforce a maximum capability in the Eth protocol.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 04:36:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4751" class=".btn">#4751</a>
            </td>
            <td>
                <b>
                    Add log to show when we've found a peer on a matching chain id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">logging</span><span class="chip">peering</span>
            </td>
            <td>
                Helpful for distinguishing between irrelevant and irrelevant peer noise in situations where we are struggling to hold onto peers from the same chain.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 04:24:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4750" class=".btn">#4750</a>
            </td>
            <td>
                <b>
                    Add Gabriel Fukushima as a maintainer
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
Proposing @gfukushima as a new Besu maintainer. They have made over 5 significant [commits](https://github.com/hyperledger/besu/pulls?q=is%3Apr+author%3Agfukushima+is%3Aclosed) that have improved the quality of Besu and/or added new features.

Voting ends 2 weeks from the publication of this PR or once more than 50% of the current maintainers approve.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.

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
        Created At 2022-11-30 03:29:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4749" class=".btn">#4749</a>
            </td>
            <td>
                <b>
                    update tuweni
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">dependencies</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <macfarla.github@gmail.com>

Update tuweni to 2.3.1

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-29 22:29:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4748" class=".btn">#4748</a>
            </td>
            <td>
                <b>
                    [WIP] Near head checkpoint sync better peering
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

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-29 13:12:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4744" class=".btn">#4744</a>
            </td>
            <td>
                <b>
                    [WORK IN PROGRESS] flat database filling pruning 
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
        Created At 2022-11-28 22:40:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4743" class=".btn">#4743</a>
            </td>
            <td>
                <b>
                    Spike transition schedule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New Timestamp Protocol Schedule Spike
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 18:47:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4742" class=".btn">#4742</a>
            </td>
            <td>
                <b>
                    Implement EIP 3860
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description
Implement EIP 3860

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 18:34:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4741" class=".btn">#4741</a>
            </td>
            <td>
                <b>
                    Removing deprecated method
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
Remove deprecated method isEqualToIgnoringGivenFields from the package org.assertj.core.api 

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
        Created At 2022-11-27 13:32:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4738" class=".btn">#4738</a>
            </td>
            <td>
                <b>
                    Fix: log jemalloc presence at startup, not at shutdown
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
        Created At 2022-11-25 10:08:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4737" class=".btn">#4737</a>
            </td>
            <td>
                <b>
                    [WORK IN PROGRESS] Preload state trie node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

Signed-off-by: Karim TAAM <karim.t2am@gmail.com>
Co-authored-by: Ameziane H <ameziane.hamlat@consensys.net>

## PR description
The idea behind this PR is to preload asynchronously account nodes and storage nodes from the database during the commit step to use these nodes during persist step.
We've created two caches, one for account nodes and one for storage nodes. The size of these caches is 100k for accounts and 200k for storage. We've tested other values but this configuration is the one that works better.
We also exporter cache metrics as Prometheus metrics to check cache efficiency.

We didn't see any impact on GC activity even on 4 GiB Heaps (-Xmx4g).

### The results
We did our tests on different AWS EC instances, here're the results. 

**M6a.xlarge** (4 vCPU, 16 GiB)
Block processing time is 34% better for median values and 41% better for 95th percentile.

<img width="1629" alt="image" src="https://user-images.githubusercontent.com/5099602/204573790-1eaad42d-2328-4282-b963-859a31ce81f7.png">


**M5.xlarge** (4 vCPU, 16 GiB)
Block processing time is 28% better for median values and 95th percentile.

<img width="1629" alt="image" src="https://user-images.githubusercontent.com/5099602/204574962-75d56150-fe13-4849-9d05-034cb1dd8343.png">


**I3.2xlarge** (8 vCPU, 61 GiB)
Block processing time is 21% better for median values and 95th percentile.

<img width="1629" alt="image" src="https://user-images.githubusercontent.com/5099602/204575720-2cf3b0da-5ab4-4a77-a20d-5d6667a042f4.png">



**Cache Efficiency**
We can see in the screenshots below that these two caches are very efficient (>99%) and increasing storage cache size more than 200k is not necessary.

Account cache size = 100k and Storage cache size = 200k
<img width="1644" alt="image" src="https://user-images.githubusercontent.com/5099602/204576899-b19496f2-5e6b-418e-8907-66f0ccedb1b1.png">

Account cache size = 100k and Storage cache size = 1 million
<img width="1644" alt="image" src="https://user-images.githubusercontent.com/5099602/204577704-98d2279d-e139-4c7b-bb70-364560274c4b.png">

  

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
        Created At 2022-11-25 09:34:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4736" class=".btn">#4736</a>
            </td>
            <td>
                <b>
                    fix typo in error message.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Bakuchi <49754494+massun-onibakuchi@users.noreply.github.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
maybe I found a typo in error message

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fix a minor typo in `NONCE_TOO_FAR_IN_FUTURE_FOR_SENDER `

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-25 05:36:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4735" class=".btn">#4735</a>
            </td>
            <td>
                <b>
                    Near head checkpoint sync
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
Add near-head checkpoint sync support

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Fixes #4573
Linked to #4703 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-25 04:21:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4733" class=".btn">#4733</a>
            </td>
            <td>
                <b>
                    [Shandong] Turn PUSH0 valid for EOF1 validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description
Shandong implements [EIP-3855](https://eips.ethereum.org/EIPS/eip-3855) (PUSH0 instruction) and must be considered as valid opcode for EOFv1 validation.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

Signed-off-by: Diego López León <dieguitoll@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 23:46:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4732" class=".btn">#4732</a>
            </td>
            <td>
                <b>
                    Fix attempt to send unsupported message (13) via cap eth/67
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
WorldStatePeerTrieNodeFinder - Do not call GetNodeData if the protocol version is greater than Eth66

## Fixed Issue(s)
fixes #4731

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 23:16:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4730" class=".btn">#4730</a>
            </td>
            <td>
                <b>
                    Implement eth/68 (EIP-5793)
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
Implement eth/68

- https://eips.ethereum.org/EIPS/eip-5793

> The NewPooledTransactionHashes message announces transaction hashes, allowing the peer to selectively fetch transactions it does not yet have.
> 
> EIP-4844 introduces a new transaction type for blob transactions. Since these blob transactions are large, naively broadcasting them to sqrt(peers) could significantly increase bandwidth requirements. Adding the transaction type and the size to the announcement message will allow nodes to select which transactions they want to fetch and also allow them to load balance or throttle peers based on past behavior.
> 
> The added metadata fields will also enable future - upgradeless - protocol tweaks to prevent certain transaction type (e.g. blob transactions) or certain transaction sizes (e.g. 128KB+) from being blindly broadcast to many peers. Enforcing announcements only and retrieval on demand would ensure a much more predictable networking behavior, limiting the amplification effect of transaction propagation DoS attack.

Modify the NewPooledTransactionHashes (0x08) message:

(eth/67): [hash_0: B_32, hash_1: B_32, ...]
(eth/68): [[type_0: B_1, type_1: B_1, ...], [size_0: B_4, size_1: B_4, ...], [hash_0: B_32, hash_1: B_32, ...]]

## Fixed Issue(s)
fixes #4715
## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 07:33:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4728" class=".btn">#4728</a>
            </td>
            <td>
                <b>
                    [Shandong] Update bootnodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description
Update Shandong boot nodes according those in the [Shandong Management Meta Issue](https://github.com/ethereumjs/ethereumjs-monorepo/issues/2375) from _ethereumjs_

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

Signed-off-by: Diego López León <dieguitoll@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-23 17:52:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4727" class=".btn">#4727</a>
            </td>
            <td>
                <b>
                    Add option to skip nonce validation on private transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

privacy-validate-private-transactions is enabled by default, but there are situations where you may want to allow the private transactions to still be processed. For instance, if you have a separate validator where the PMT is valid, but the validator doesn't know the private transaction is invalid.

Enabling this option could potentially cause your private state to diverge from one another. If you wish to enable this option it is recommended that you re-sync all nodes your network after you do so. 

## Fixed Issue(s)
Some mitigation for https://github.com/hyperledger/besu/issues/614
Fixes https://github.com/hyperledger/besu/issues/1942

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-23 16:46:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4726" class=".btn">#4726</a>
            </td>
            <td>
                <b>
                    [Shandong] EIP-3860 support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description
Shandong supports [EIP-3860](https://eips.ethereum.org/EIPS/eip-3860) and the first block to fail without this is [block 188](https://explorer.shandong.ethdevops.io/block/188)

As with the other calculators, the testing is expected to be part of the [ethereum/tests](https://github.com/ethereum/tests) suite. 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).

Signed-off-by: Diego López León <dieguitoll@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-23 15:24:23 +0000 UTC
    </div>
</div>

