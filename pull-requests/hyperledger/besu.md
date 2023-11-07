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
                PR <a href="https://github.com/hyperledger/besu/pull/6138" class=".btn">#6138</a>
            </td>
            <td>
                <b>
                    Bws badblock oom
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6121" class=".btn">#6121</a>
            </td>
            <td>
                <b>
                    5571migrate tests to junit5
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
issue #5571 
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-05 00:10:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6119" class=".btn">#6119</a>
            </td>
            <td>
                <b>
                    Update RPCs for yParity
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

* Update the GraphQL and JSON-RPC endpoints to provide `yParity` instead of `v` for non-legacy transactions.
* Update the JSON-RPC tests to use the Hive data. 
* Add JSON-RPC tests for Shanghai and Cancun blocks/fields.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 17:29:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6117" class=".btn">#6117</a>
            </td>
            <td>
                <b>
                    clean up the ProcessableBlockHeader
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This removes a few fields that don't make sense and that are not used in the existing core/ProcessableBlockHeader class. 
This introduces a interface ProcessableBlockHeader in the plugin module.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 03:43:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6116" class=".btn">#6116</a>
            </td>
            <td>
                <b>
                    Pipeline for debug RPC endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Increase efficiency by using pipeline for debug block endpoints

Refs #5322 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 02:20:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6114" class=".btn">#6114</a>
            </td>
            <td>
                <b>
                    Reference Tests v13
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

v13 of the official Ethereum Reference Tests.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 15:06:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6110" class=".btn">#6110</a>
            </td>
            <td>
                <b>
                    [MINOR] - Add 23.10.1 correct changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add 23.10.1 final changelog

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-01 03:36:16 +0000 UTC
    </div>
</div>

