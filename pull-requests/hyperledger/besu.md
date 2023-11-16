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
                PR <a href="https://github.com/hyperledger/besu/pull/6174" class=".btn">#6174</a>
            </td>
            <td>
                <b>
                    [MINOR] Eth peer toString() improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * only include peer id in the peer.toString() method (remove from peerConnection)
* only log enode not id also
fixes #6169 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-16 03:34:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6172" class=".btn">#6172</a>
            </td>
            <td>
                <b>
                    Changelog23.10.2
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
        Created At 2023-11-15 16:26:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6171" class=".btn">#6171</a>
            </td>
            <td>
                <b>
                    uprev to 23.10.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                finishes out 23.10.2 release
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 14:38:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6168" class=".btn">#6168</a>
            </td>
            <td>
                <b>
                    Fix EthFeeHistory reward calculation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">TeamRevenant</span><span class="chip">mainnet</span><span class="chip">RPC</span>
            </td>
            <td>
                ### Description
fixes: #6170 
eth_feeHistory returns wrong rewards. The following request on Sepolia returns: 

```
{
   "jsonrpc":"2.0",
   "method":"eth_feeHistory",
   "params":[
      "0x5",
      "0x3FA351",
      [
         0,
         20,
         30,
         100
      ]
   ],
   "id":1
}
```

Expected Result (Green) / Actual Result (red): 
```diff
{
  "baseFeePerGas": [
    "0x76c73ce5",
    "0x7e1f5d40",
    "0x7f8aed3c",
    "0x77be8999",
    "0x68c6b866",
    "0x6716f547"
  ],
  "gasUsedRatio": [
    0.7473261666666666,
    0.5450408333333333,
    0.2554263333333333,
    0,
    0.43561246666666664
  ],
  "oldestBlock": "0x3fa34d",
  "reward": [
    [
-     "0x27c9",
-     "0x27c9",
-     "0x27c9",
-     "0x27c9"
+     "0x27c9",
+     "0x77359400",
+     "0x77359400",
+     "0x1660f131b"
    ],
    [
-     "0x27c9",
-     "0x27c9",
-     "0x27c9",
-     "0x27c9"
+     "0x27c9",
+     "0x59682f00",
+     "0x59682f00",
+     "0x15eb6f2c0"
    ],
    [
-     "0x0",
-     "0x0",
-     "0x0",
-     "0x27c9"
+     "0x0",
+     "0x27c9",
+     "0x5f5e100",
+     "0x15d4b62c4"
    ],
    [
      "0x0",
      "0x0",
      "0x0",
      "0x0"
    ],
    [
-     "0x0",
-     "0x0",
-     "0x0",
-     "0x27c9"
+     "0x0",
+     "0x27c9",
+     "0xe00ac48",
+     "0x43f510f9a"
    ]
  ]
}
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-15 02:38:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6166" class=".btn">#6166</a>
            </td>
            <td>
                <b>
                    parallelisation tweaks for CI acceptance tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                TLDR: 3 x reduction in CI credit usage [~5,000](https://app.circleci.com/insights/github/hyperledger/besu/workflows/default/overview?branch=pull%2F6166&reporting-window=last-24-hours), other recent PRs [~15,000](https://app.circleci.com/insights/github/hyperledger/besu/workflows/default/overview?branch=pull%2F6156)
More insights [recent PR runs](https://app.circleci.com/insights/github/hyperledger/besu/workflows/default/overview?branch=b1d8acd4-8701-4c76-8a87-7ff2320aa95f&reporting-window=last-24-hours)

Modifications in this PR: 
* remove parallelism for acceptanceTestsCliqueBft and acceptanceTestsPermissioning and reduce the machine executor size requirement (time before: 3 min, 6 min; after: 6 min, 10 min)
* reduce parallelism for acceptanceTests task (this task failed with concurrency limit reached when parallelism was removed altogether https://app.circleci.com/pipelines/github/hyperledger/besu/25171/workflows/a5b6d9bc-fa7c-4e59-aac2-985f642492e9/jobs/164393) (parallelisation before: 4; after: 2 | time before: 4 min; after: 6 min)
* move privacy ATs to nightly build and reduce parallelism (many tests failed when parallelisation was removed https://app.circleci.com/pipelines/github/hyperledger/besu/25170/workflows/81fc005b-6f3a-4c78-a8e9-f35e6f349aa6/jobs/164381) - note there's a separate effort to remove the docker dependency used by container tests - draft PR https://github.com/hyperledger/besu/pull/5968
* remove small executor since it's not used
* added comments to explain where the machine xl executor is actually required and why
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-14 00:12:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6165" class=".btn">#6165</a>
            </td>
            <td>
                <b>
                    make sure closure is checking the protocol schedule correctly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #6164 which had a stale handle to the protocol spec after going async
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-13 21:23:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6163" class=".btn">#6163</a>
            </td>
            <td>
                <b>
                    Transactions that takes too long to evaluate, during block creation, are dropped from the txpool
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

In PR #6044, a timeout has been introduced to avoid that the transactions selection, during block creation, could take an indefinite amount of time, this PR iterates on it checking if the tx that was evaluating when the timeout occurred, took longer that the max amount of time allocated for the block creation, and if this was the case, the tx is removed from the pool, to avoid that it will be retried in future block creations.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-13 14:02:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6161" class=".btn">#6161</a>
            </td>
            <td>
                <b>
                    Tracing private transactions feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
PR for adding priv_traceTransaction API

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5280
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-12 04:50:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6159" class=".btn">#6159</a>
            </td>
            <td>
                <b>
                    reftest updates
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
        Created At 2023-11-11 02:12:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6156" class=".btn">#6156</a>
            </td>
            <td>
                <b>
                    Add `rpc-gas-cap` via transaction simulator
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
This PR adds `rpc-gas-cap` directly into the transaction simulator, which seems a better approach than the one used in #6130.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #6042 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-10 18:47:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6155" class=".btn">#6155</a>
            </td>
            <td>
                <b>
                    Release 23.10.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.10.2

### Breaking Changes
- TX pool eviction in the legacy TX pool now favours keeping oldest transactions (more likely to evict higher nonces, less likely to introduce nonce gaps) [#6106](https://github.com/hyperledger/besu/pull/6106) and [#6146](https://github.com/hyperledger/besu/pull/6146)

### Deprecations

### Additions and Improvements
- Ethereum Classic Spiral network upgrade [#6078](https://github.com/hyperledger/besu/pull/6078)
- Add a method to read from a `Memory` instance without altering its inner state [#6073](https://github.com/hyperledger/besu/pull/6073)
- TraceService: return results for transactions in block [#6086](https://github.com/hyperledger/besu/pull/6086)
- Accept `input` and `data` field for the payload of transaction-related RPC methods [#6094](https://github.com/hyperledger/besu/pull/6094)
- Add APIs to set and get the min gas price a transaction must pay for being selected during block creation [#6097](https://github.com/hyperledger/besu/pull/6097)
- TraceService: return results for transactions in block [#6086](https://github.com/hyperledger/besu/pull/6086)
- New option `--min-priority-fee` that sets the minimum priority fee a transaction must meet to be selected for a block. [#6080](https://github.com/hyperledger/besu/pull/6080) [#6083](https://github.com/hyperledger/besu/pull/6083)
- Implement new `miner_setMinPriorityFee` and `miner_getMinPriorityFee` RPC methods [#6080](https://github.com/hyperledger/besu/pull/6080)
- Clique config option `createemptyblocks` to not create empty blocks [#6082](https://github.com/hyperledger/besu/pull/6082)
- Upgrade EVM Reference Tests to v13 (Cancun) [#6114](https://github.com/hyperledger/besu/pull/6114)
- Add `yParity` to GraphQL and JSON-RPC for relevant querise. [6119](https://github.com/hyperledger/besu/pull/6119)
- Force tx replacement price bump to zero when zero base fee market is configured or `--min-gas-price` is set to 0. This allows for easier tx replacement in networks where there is not gas price. [#6079](https://github.com/hyperledger/besu/pull/6079)
- Introduce the possibility to limit the time spent selecting pending transactions during block creation, using the new experimental option `Xblock-txs-selection-max-time` on PoS and PoW networks (by default set to 5000ms) or `Xpoa-block-txs-selection-max-time` on PoA networks (by default 75% of the min block time) [#6044](https://github.com/hyperledger/besu/pull/6044)

### Bug fixes
- Upgrade netty to address CVE-2023-44487, CVE-2023-34462 [#6100](https://github.com/hyperledger/besu/pull/6100)
- Upgrade grpc to address CVE-2023-32731, CVE-2023-33953, CVE-2023-44487, CVE-2023-4785 [#6100](https://github.com/hyperledger/besu/pull/6100)
- Fix blob gas calculation in reference tests [#6107](https://github.com/hyperledger/besu/pull/6107)
- Limit memory used in handling invalid blocks [#6138](https://github.com/hyperledger/besu/pull/6138)

---


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-10 17:59:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6154" class=".btn">#6154</a>
            </td>
            <td>
                <b>
                    update version for snapshot
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
        Created At 2023-11-10 16:35:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6152" class=".btn">#6152</a>
            </td>
            <td>
                <b>
                    Gas price pending TX test using wrong class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Create instance of the correct class in gas price TX test

## Fixed Issue(s)
No issue raised for this
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-10 13:03:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6151" class=".btn">#6151</a>
            </td>
            <td>
                <b>
                    fix yParity flakey test
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

Fix the flakiness in EthGetTransactionByHashTest as well as some other sonar identified cleanup.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 21:52:32 +0000 UTC
    </div>
</div>

