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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6150" class=".btn">#6150</a>
            </td>
            <td>
                <b>
                    Clamp up-front gas calculation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Clamp upfront gas calculations to uint256 max instead of throwing an exception. Fix related encoding changes and tests to validate.

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
        Created At 2023-11-09 16:09:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6148" class=".btn">#6148</a>
            </td>
            <td>
                <b>
                    Remove LowestInvalidNonceCache
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

LowestInvalidNonceCache was introduce in #4425, as a workaround for avoiding that non executable txs fill the txpool, while we were implementing an better solution to the problem, that become the new layered txpool that is now the default option in Besu, and is tailored for public network.
At this point we can make the simple legacy txpool more private network friendly, and the LowestInvalidNonceCache is usually creating issues these networks, so it makes sense to remove this workaround, since there should be less risk of spammy txs there, and in case users can always switch to layered.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #6058 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 14:21:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6147" class=".btn">#6147</a>
            </td>
            <td>
                <b>
                    Cached blob txs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #6025 

- adds LRU cache to retain blobs for 3 epochs in case of re-orgs so they can be restored to tx pool for future inclusion.
- worst case memory usage would be around 77MB on heap
- adds means for Transaction.Builder to copy an immutable Transaction
- upgrades errorprone, checkerframework, and caffine
- miscellaneous sonar fixes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 13:39:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6146" class=".btn">#6146</a>
            </td>
            <td>
                <b>
                    Apply the same reverse sort order as https://github.com/hyperledger/b…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
PR https://github.com/hyperledger/besu/pull/6106 reversed the transaction sort order, but only for the gas-price sorter.

This PR applies the same logic to the base-fee sorter.

FYI @fab-10 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 10:43:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6143" class=".btn">#6143</a>
            </td>
            <td>
                <b>
                    Synchronize access to block header
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
As outlined in the comment in https://github.com/hyperledger/besu/issues/6140 it appears to be the case that access to the block header isn't thread safe when the block being requested is a newly added chain head.

## Fixed Issue(s)
Fixes #6140 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 10:32:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6138" class=".btn">#6138</a>
            </td>
            <td>
                <b>
                    Backward sync invalid block causes Out of Memory error
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
Besu fails to import a block due to an invalid block error during BWS and then fails with an OutOfMemoryError.

The fix is to limit the included blocks and block headers in the `onBadChain` event. I have set the limit to be the same as what is set for the maximum number of entries cached in the `BadBlockManager`. The `BadBlockManager` is currently the only listener for this event and the limit of 100 also seems reasonable for the `onBadChain` event.

### Heap dump analysis
![image (1)](https://github.com/hyperledger/besu/assets/909467/bcb2e0b7-bc43-460c-a5be-a3134f018ca9)

![image (2)](https://github.com/hyperledger/besu/assets/909467/5fd48a0f-c075-476a-b2b7-e753a9debbc3)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #6118 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 06:34:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6137" class=".btn">#6137</a>
            </td>
            <td>
                <b>
                    Revert "Discard invalid transaction" warning logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts part of the logging changes in #6127 

On a public network transactions are dropped for a variety of reasons and very frequently, and this blows the logs up.  E.g.:
```
{"@timestamp":"2023-11-07T00:05:18,003","level":"WARN","thread":"nioEventLoopGroup-3-9","class":"TransactionPool","message":"Discard invalid transaction 0x3124130967cb066ab9a6c5807a96f3147d354ae09f1bb8cda6b95c39033756f1={MessageCall, 51156, 0xa76a91f8b0d7ef28d2b76a703bc0770ba8996bfc, EIP1559, mf: 12 wei, pf: 2 wei, gl: 800000, v: 0 wei, to: 0x9d51bca23612851f98ced6d4f7aac75356d45f58}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:18,004","level":"WARN","thread":"nioEventLoopGroup-3-9","class":"TransactionPool","message":"Discard invalid transaction 0x5549d54c0b7025b4ba0f38ae06df73ee2e3eb70d2b8865216c136df3d0779d71={MessageCall, 51157, 0xa76a91f8b0d7ef28d2b76a703bc0770ba8996bfc, EIP1559, mf: 12 wei, pf: 2 wei, gl: 800000, v: 0 wei, to: 0x9d51bca23612851f98ced6d4f7aac75356d45f58}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:18,004","level":"WARN","thread":"nioEventLoopGroup-3-9","class":"TransactionPool","message":"Discard invalid transaction 0x97b1abe588275c401407c4c77146bfed484cac7d262baf3902239ed1df2205c1={MessageCall, 51158, 0xa76a91f8b0d7ef28d2b76a703bc0770ba8996bfc, EIP1559, mf: 12 wei, pf: 2 wei, gl: 800000, v: 0 wei, to: 0x9d51bca23612851f98ced6d4f7aac75356d45f58}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:18,004","level":"WARN","thread":"nioEventLoopGroup-3-9","class":"TransactionPool","message":"Discard invalid transaction 0xab615870b1fa53c6d3259e537b90c0fdbc171037b60586c9145c669dbd7df115={MessageCall, 51159, 0xa76a91f8b0d7ef28d2b76a703bc0770ba8996bfc, EIP1559, mf: 12 wei, pf: 2 wei, gl: 800000, v: 0 wei, to: 0x9d51bca23612851f98ced6d4f7aac75356d45f58}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:18,004","level":"WARN","thread":"nioEventLoopGroup-3-9","class":"TransactionPool","message":"Discard invalid transaction 0x56c5a492629efd144aca16ef57c21455bd0685d4fd91e2f19ab8f8321c8e84c3={MessageCall, 51160, 0xa76a91f8b0d7ef28d2b76a703bc0770ba8996bfc, EIP1559, mf: 12 wei, pf: 2 wei, gl: 800000, v: 0 wei, to: 0x9d51bca23612851f98ced6d4f7aac75356d45f58}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:18,004","level":"WARN","thread":"nioEventLoopGroup-3-9","class":"TransactionPool","message":"Discard invalid transaction 0xce7da2376d040fb5b5463430558437ddd09126908087afc376ba6b98ed1f6dfb={MessageCall, 51161, 0xa76a91f8b0d7ef28d2b76a703bc0770ba8996bfc, EIP1559, mf: 12 wei, pf: 2 wei, gl: 800000, v: 0 wei, to: 0x9d51bca23612851f98ced6d4f7aac75356d45f58}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:18,004","level":"WARN","thread":"nioEventLoopGroup-3-9","class":"TransactionPool","message":"Discard invalid transaction 0x99c1928d6df041948b4f0e86f7e081562880237d5bc5136446ab70db02be791f={MessageCall, 51162, 0xa76a91f8b0d7ef28d2b76a703bc0770ba8996bfc, EIP1559, mf: 12 wei, pf: 2 wei, gl: 800000, v: 0 wei, to: 0x9d51bca23612851f98ced6d4f7aac75356d45f58}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:18,084","level":"WARN","thread":"EthScheduler-Transactions-0","class":"TransactionPool","message":"Discard invalid transaction 0xcd3fab021ba2cb0022c71e873c87fcc44b5eca17bea6874bf9845f8e9f52080b={MessageCall, 12074, 0x6b78b7c287b21d4d65cb91bd84eb6b79ab9e8af5, EIP1559, mf: 24 wei, pf: 2 wei, gl: 31628, v: 0 wei, to: 0xff00000000000000000000000000000000000000}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:18,084","level":"WARN","thread":"EthScheduler-Transactions-0","class":"TransactionPool","message":"Discard invalid transaction 0xd5ffddbae76a7cf76e8a14ca88ae8cd1146758bc2b849406964b365cbfe8d9fb={MessageCall, 43067, 0xe02c9aef141d5bbf78fb20c5d46da5faa635cef7, EIP1559, mf: 24 wei, pf: 2 wei, gl: 26012, v: 0 wei, to: 0xff00000000000000000000000000000000042069}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:18,589","level":"WARN","thread":"EthScheduler-Transactions-0","class":"TransactionPool","message":"Discard invalid transaction 0x7b2183566b34e459f665df56d2173e0f295755db1a3384e46d5437b23ac9f014={MessageCall, 152692, 0x39b9c34ee948752e640cd01364036dc8468416b8, EIP1559, mf: 24 wei, pf: 2 wei, gl: 31000, v: 0 wei, to: 0xff00000000000000000000000000000000042069}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:18,911","level":"WARN","thread":"EthScheduler-Transactions-0","class":"TransactionPool","message":"Discard invalid transaction 0x541895f95660f310606b554c26b6ce02cd11472d4bdde32543705c0aa371ec26={MessageCall, 0, 0x4fa8acbc72b834f5976a75f917f66c384b3e09a9, FRONTIER, gp: 15 wei, gl: 21000, v: 114.65 finney, to: 0x3fdf957b0054d1617132d4d874eb41d4efe81cff}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:19,001","level":"WARN","thread":"nioEventLoopGroup-3-9","class":"TransactionPool","message":"Discard invalid transaction 0x0309aa802e467da5a1cce6d7c52cf3553f897c58c98f52aae21bc0c41c501c3f={MessageCall, 58315, 0x046f8def6dba949b2e588a67bfa14faef584dfc4, EIP1559, mf: 19 wei, pf: 2 wei, gl: 800000, v: 0 wei, to: 0x117a5ab00f93469bea455f0864ef9ad8d9630cc9}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:19,002","level":"WARN","thread":"nioEventLoopGroup-3-9","class":"TransactionPool","message":"Discard invalid transaction 0x0ed8048bb4886786d1099089e1a735249cbe0c9f993d468d91d746d6d82846ad={MessageCall, 58322, 0x046f8def6dba949b2e588a67bfa14faef584dfc4, EIP1559, mf: 19 wei, pf: 2 wei, gl: 800000, v: 0 wei, to: 0x117a5ab00f93469bea455f0864ef9ad8d9630cc9}, reason GAS_PRICE_TOO_LOW","throwable":""}
{"@timestamp":"2023-11-07T00:05:19,229","level":"WARN","thread":"EthScheduler-Transactions-0","class":"TransactionPool","message":"Discard invalid transaction 0x7aef4bc36c4a77f421f9a487bbcdca35b465ecd4a0a6f01a65e7ed1abe5fa1ec={MessageCall, 270917, 0xbaec44f49df3578749fb299769d723eaccddb605, EIP1559, mf: 24 wei, pf: 2 wei, gl: 26620, v: 0 wei, to: 0xff00000000000000000000000000000000042069}, reason GAS_PRICE_TOO_LOW","throwable":""}
```

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
        Created At 2023-11-07 00:29:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6135" class=".btn">#6135</a>
            </td>
            <td>
                <b>
                    Make the tracer used for block building block aware
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
The changes in this PR make the tracer that is used during block building block aware. 

This PR also adds a new method to the BlockAwareOperationTracer, that is called at the beginning of building a new block. 

The tracer used during the block building can be provided by the PluginTransactionSelector.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 23:29:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6130" class=".btn">#6130</a>
            </td>
            <td>
                <b>
                    Add `rpc-gas-cap` to CLI options
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
This PR introduces the CLi option`rpc-gas-cap` which allows users to limit the amount of gas used by the  RPC methods `eth_call` and `eth_getEstimateGas`. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #6042 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 14:47:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6127" class=".btn">#6127</a>
            </td>
            <td>
                <b>
                    Log missing chain head as warning, not trace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Change `CHAIN_HEAD_NOT_AVAILABLE` to a warning, not a trace log entry

## Fixed Issue(s)
Fixes #6126 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 11:02:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6122" class=".btn">#6122</a>
            </td>
            <td>
                <b>
                    [#5561]migrate tests to junit5
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
        Created At 2023-11-05 02:36:32 +0000 UTC
    </div>
</div>

