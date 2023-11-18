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
                PR <a href="https://github.com/hyperledger/besu/pull/6183" class=".btn">#6183</a>
            </td>
            <td>
                <b>
                    Revert "fix tests collisions"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit ee7c22ca8b6f591e378b5cec34f2289b1711490e.

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This change from the bonsai reference test worldstate pr #5686 seems to be causing a regression on goerli for block [#9727365](https://goerli.etherscan.io/block/9727365)


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-18 07:03:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6181" class=".btn">#6181</a>
            </td>
            <td>
                <b>
                    just test
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
        Created At 2023-11-17 12:17:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6179" class=".btn">#6179</a>
            </td>
            <td>
                <b>
                    Stretch timeout when low peer count
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                in low peer count networks, be more lenient with timeout and useless response disconnects
Also reset all timeouts not just the specific messageCode
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-17 04:46:52 +0000 UTC
    </div>
</div>

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

