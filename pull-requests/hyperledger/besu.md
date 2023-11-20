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
                PR <a href="https://github.com/hyperledger/besu/pull/6187" class=".btn">#6187</a>
            </td>
            <td>
                <b>
                    consider peer reputation score when deciding to disconnect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">peering</span>
            </td>
            <td>
                Noticed in peering logs we are disconnecting quite useful peers with timeouts and "useless responses". This exacerbates peering issues because we are quite early to disconnect, whereas if we just wait a bit longer the peer can still be useful. More of an issue in low peer count networks. 
* consider peer reputation score when deciding whether to disconnect peer for repeated timeouts/useless responses
* increase threshold for timeout counts
* decrease score points deducted for timeout/useless response


```
➜  besu grep  "Disconnect - Outbound" besu03.log
2023-11-17 17:47:27.730+10:00 | nioEventLoopGroup-3-5 | DEBUG | EthProtocolManager | Disconnect - Outbound - 0x0b TIMEOUT - 0x45d5... - 5 peers left
2023-11-17 17:49:10.232+10:00 | nioEventLoopGroup-3-1 | DEBUG | EthProtocolManager | Disconnect - Outbound - 0x0b TIMEOUT - 0xcbba... - 4 peers left
2023-11-17 18:02:33.476+10:00 | nioEventLoopGroup-3-8 | DEBUG | EthProtocolManager | Disconnect - Outbound - 0x03 USELESS_PEER - 0x6a7... - 3 peers left
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 05:47:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6186" class=".btn">#6186</a>
            </td>
            <td>
                <b>
                    comment out flaky part of acceptance test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">flake</span>
            </td>
            <td>
                this particular test is flaky. There are other tests for the same class that work more reliably. 

Example of flaky fail -
https://app.circleci.com/pipelines/github/hyperledger/besu/25195/workflows/a5a40b6e-0f1d-4ac3-87e6-108bcce92b9e/jobs/164640
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 05:41:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6185" class=".btn">#6185</a>
            </td>
            <td>
                <b>
                    Add Experimental RockDB Subcommand for printing usage per column family
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pretty much a lift and shift of @ahamlat's https://github.com/ahamlat/RocksdDB-Column-Families-Size

```
➜  besu git:(rocksdb-usage-subcommand) $BESU storage x-rocksdb usage --help
Usage: besu storage x-rocksdb usage [-hV]
Prints disk usage
  -h, --help      Show this help message and exit.
  -V, --version   Print version information and exit.
  
➜  besu git:(rocksdb-usage-subcommand) $BESU storage x-rocksdb --help
Usage: besu storage x-rocksdb [-hV] [COMMAND]
Print RocksDB information
  -h, --help      Show this help message and exit.
  -V, --version   Print version information and exit.
Commands:
  usage  Prints disk usage
```

```
$BESU --data-path=/tmp/besu storage x-rocksdb usage
****** Column family 'BLOCKCHAIN' size: 7 KiB ******
Number of keys : 70
Number of live snapshots : 0
Total size of SST Files : 4 KiB
Size of live SST Filess : 4 KiB
Column family size (with getColumnFamilyMetaData) : 4 KiB

****** Column family 'ACCOUNT_INFO_STATE' size: 1 KiB ******
Number of keys : 2
Number of live snapshots : 0
Total size of SST Files : 1 KiB
Size of live SST Filess : 1 KiB
Column family size (with getColumnFamilyMetaData) : 1 KiB

****** Column family 'TRIE_BRANCH_STORAGE' size: 1 KiB ******
Number of keys : 7
Number of live snapshots : 0
Total size of SST Files : 2 KiB
Size of live SST Filess : 2 KiB
Column family size (with getColumnFamilyMetaData) : 2 KiB

****** Column family 'TRIE_LOG_STORAGE' size: 5 KiB ******
Number of keys : 103
Number of live snapshots : 0
Total size of SST Files : 7 KiB
Size of live SST Filess : 7 KiB
Column family size (with getColumnFamilyMetaData) : 7 KiB

****** Column family 'VARIABLES' size: 1 KiB ******
Number of keys : 6
Number of live snapshots : 0
Total size of SST Files : 2 KiB
Size of live SST Filess : 2 KiB
Column family size (with getColumnFamilyMetaData) : 2 KiB
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 02:05:08 +0000 UTC
    </div>
</div>

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

