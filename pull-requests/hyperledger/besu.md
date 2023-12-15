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
                PR <a href="https://github.com/hyperledger/besu/pull/6303" class=".btn">#6303</a>
            </td>
            <td>
                <b>
                    Add --X-trie-log subcommand
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
This is a more direct approach to the previous attempt in #6188.
Tests showed that the previous attempt was taking too long (3 hours) to prune a 3.5 months old.

In this PR we "reset" the cf and load only the trielogs that we want to retain in the DB.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Part of #5390 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 04:10:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6302" class=".btn">#6302</a>
            </td>
            <td>
                <b>
                    Disable txpool during fullsync
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
        Created At 2023-12-14 15:52:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6300" class=".btn">#6300</a>
            </td>
            <td>
                <b>
                    create trie package for bonsai and forest
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

A PR to place Bonsai and Forest in the same trie package. This PR is a preparation for the introduction of Verkle. This trie package will have Verkle in a next PR and we will add a common package so that the different trie substructures can share classes if needed. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 10:58:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6299" class=".btn">#6299</a>
            </td>
            <td>
                <b>
                    [MINOR] Trailing peer limit log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">logging</span>
            </td>
            <td>
                fixes #6269 

```
sallymacfarlane@dev-elc-besu-teku-mainnet-dev-sally-trailing-peer-log-3:/var/log/besu$ grep Trailing besu.log
{"@timestamp":"2023-12-14T12:50:11,138","level":"DEBUG","thread":"nioEventLoopGroup-3-5","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xadb935a416b0c19aaf... with height 18783177","throwable":""}
{"@timestamp":"2023-12-14T12:51:47,696","level":"DEBUG","thread":"nioEventLoopGroup-3-9","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xc8a80e895f6b85f8ff... with height 18299999","throwable":""}
{"@timestamp":"2023-12-14T12:51:49,471","level":"DEBUG","thread":"nioEventLoopGroup-3-1","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0x48f462dab313723e05... with height 18001000","throwable":""}
{"@timestamp":"2023-12-14T12:52:19,523","level":"DEBUG","thread":"nioEventLoopGroup-3-5","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13883323","throwable":""}
{"@timestamp":"2023-12-14T12:52:40,702","level":"DEBUG","thread":"nioEventLoopGroup-3-4","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13885662","throwable":""}
{"@timestamp":"2023-12-14T12:52:49,897","level":"DEBUG","thread":"nioEventLoopGroup-3-2","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13886842","throwable":""}
{"@timestamp":"2023-12-14T12:53:19,501","level":"DEBUG","thread":"nioEventLoopGroup-3-9","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13889692","throwable":""}
{"@timestamp":"2023-12-14T12:53:49,340","level":"DEBUG","thread":"nioEventLoopGroup-3-3","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13891310","throwable":""}
{"@timestamp":"2023-12-14T12:54:19,841","level":"DEBUG","thread":"nioEventLoopGroup-3-10","class":"TrailingPeerLimiter","message":"Enforcing trailing peers limit (min height 18784339, max trailing peers 0) by disconnecting 0xd9c1f1b8c84f4dcd96... with height 13893155","throwable":""}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 09:20:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6297" class=".btn">#6297</a>
            </td>
            <td>
                <b>
                    [MINOR] add genesis file name to config overview
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span><span class="chip">ux</span><span class="chip">non mainnet (private networks)</span>
            </td>
            <td>
                ```
# Configuration:                                                                                   #
# Network: Custom genesis file                                                                     #
# /Users/sm/workspace/besu/config/besu/genesis-linea.json                                          #
# Network Id: 59140                                                                                #
# Data storage: Forest                                                                             #
# Sync mode: Snap                                                                                  #
# RPC HTTP APIs: ADMIN,ETH,NET,WEB3,PERM,DEBUG,MINER,EEA,PRIV,TXPOOL                               #
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 06:32:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6296" class=".btn">#6296</a>
            </td>
            <td>
                <b>
                    [MINOR] Remove vintage engine dependencies where unused
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                Remove the junit-vintage-engine dependency from several modules where it's not used
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 05:29:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6295" class=".btn">#6295</a>
            </td>
            <td>
                <b>
                    Snap sync client handle empty final account storage ranges
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

Bugfix snap sync edge case.  When snap syncing large contract storage, if the final requested range is empty, but there is an accompanying proof of exclusion, besu will not mark the request complete and will endlessly retry.

This PR handles this case by marking the request complete as long as there is an accompanying proof

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 22:41:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6293" class=".btn">#6293</a>
            </td>
            <td>
                <b>
                    move forest class to a specific package
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

This PR prepares for the introduction of the Verkle trie code. I start by cleaning up the worldstate section, moving and renaming everything that is forest into a specific package in order to clarify the difference between Bonsai and Forest in the code.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 14:55:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6289" class=".btn">#6289</a>
            </td>
            <td>
                <b>
                    Store trielog as blobdb
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
Store trielog as blobdb to improve performance.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See https://github.com/hyperledger/besu/issues/5866
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 07:49:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6288" class=".btn">#6288</a>
            </td>
            <td>
                <b>
                    [MINOR] Include Enode URL in error message if parsing exception
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                eg in bootnodes config

Before

2023-12-13 12:08:50.949+10:00 | main | ERROR | Besu | Failed to start Besu Invalid IP address (or DNS query resolved an invalid IP). --Xdns-enabled is true but --Xdns-update-enabled flag is false.


After

2023-12-13 12:11:14.581+10:00 | main | ERROR | Besu | Failed to start Besu Invalid IP address 'enode://bob@bob:8000' (or DNS query resolved an invalid IP). --Xdns-enabled is true but --Xdns-update-enabled flag is false.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 02:11:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6287" class=".btn">#6287</a>
            </td>
            <td>
                <b>
                    Increase scope of reference tests
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

Add new forks to transaction tests, add bad rlp to rlp ref tests.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 22:20:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6286" class=".btn">#6286</a>
            </td>
            <td>
                <b>
                    Release candidate 3 for 23.10.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 20:40:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6285" class=".btn">#6285</a>
            </td>
            <td>
                <b>
                    Add trace to web socket JSON/RPC responses
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Trace WS JSON/RPC responses (successes and failures)

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/6276

## Example trace output

Successful `eth_getBlockByNumber`:

```
2023-12-12 10:43:41.553+00:00 | vert.x-eventloop-thread-1 | TRACE | WebSocketMessageHandler | {"jsonrpc":"2.0","id":51,"result":{"number":"0x0","hash":"0x74f92c171677a9f8b1eac53fc4f2c2e0d6bbc7a7b9b259fd0067f7b573951e16","mixHash":"0x63746963616c2062797a616e74696e65206661756c7420746f6c6572616e6365","parentHash":"0x0000000000000000000000000000000000000000000000000000000000000000","nonce":"0x0000000000000000","sha3Uncles":"0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347","logsBloom":"0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000","transactionsRoot":"0x56e81f171bcc55a6ff8345e692c0f86e5b48e01b996cadc001622fb5e363b421","stateRoot":"0x56e81f171bcc55a6ff8345e692c0f86e5b48e01b996cadc001622fb5e363b421","receiptsRoot":"0x56e81f171bcc55a6ff8345e692c0f86e5b48e01b996cadc001622fb5e363b421","miner":"0x0000000000000000000000000000000000000000","difficulty":"0x1","totalDifficulty":"0x1","extraData":"0xf88fa00000000000000000000000000000000000000000000000000000000000000000f869945c9437de876531c73c9618d13872f7508869f2539474474cf92e9b74df7a2ce2c4fbc0830c773b7a769462f241db855d439cc79f5d2bd4a58eeb9c5d01cd946d544f03911b74425dd4112e95f93b82ac6302f19477fd5cb2aea0b91e7e4faf7625bf9dbaee39ee47c080c0","size":"0x292","gasLimit":"0x1fffffffffffff","gasUsed":"0x0","timestamp":"0x58ee40ba","uncles":[],"transactions":[]}}

```

Failed `eth_getBlockByNumber`:

```
2023-12-12 10:44:02.881+00:00 | vert.x-eventloop-thread-1 | TRACE | WebSocketMessageHandler | {"jsonrpc":"2.0","id":51,"error":{"code":-32602,"message":"Invalid params"}}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 10:47:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6284" class=".btn">#6284</a>
            </td>
            <td>
                <b>
                    [#6201] Duplicate "Terminating connection" message on peer connections
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
There are two invocations to the method "terminateConnection" (ApiHandler and NettyPeerConnection). In the case of NettyPeerConnection it is called inside a listener.
The correct thing is to control that the terminateConnection method is executed once even if it is called several times.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#6201
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 08:54:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6283" class=".btn">#6283</a>
            </td>
            <td>
                <b>
                    [MINOR] More cli tests to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">TeamRevenant</span>
            </td>
            <td>
                builds on #6281 and #6282 
refs #5571 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 08:09:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6282" class=".btn">#6282</a>
            </td>
            <td>
                <b>
                    [MINOR] CLI Subcommands migrate to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">TeamRevenant</span>
            </td>
            <td>
                builds on #6281 

refs #5571 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 07:37:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6281" class=".btn">#6281</a>
            </td>
            <td>
                <b>
                    [MINOR] CLI unit tests migrate to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">TeamRevenant</span>
            </td>
            <td>
                refs #5571 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 04:04:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6280" class=".btn">#6280</a>
            </td>
            <td>
                <b>
                    [MINOR] migrate remaining Crypto tests to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                fixes #5568 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 22:52:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6278" class=".btn">#6278</a>
            </td>
            <td>
                <b>
                    bulk update of ATs to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                test to see if updating all at once avoids the gradle error encountered in #6262 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 21:01:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6275" class=".btn">#6275</a>
            </td>
            <td>
                <b>
                    Update Gradle plugins and replace unmaintained license plugin
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

Update all the Gradle plugins to their latest version, and replace the unmaintained `hierynomus.license` plugin with the actively maintained [Gradle License Report](https://github.com/jk1/Gradle-License-Report).
There are also few GHA Gradle cache optimizations.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 16:09:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6274" class=".btn">#6274</a>
            </td>
            <td>
                <b>
                    Sequenced pool synonym for legacy pool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Introduces the new `sequenced` synonym for the `legacy` transaction pool, as discussed in https://github.com/hyperledger/besu/issues/6211.

The PR adds enough for users to start switching to the `--tx-pool=sequenced` option ahead of removal of the `legacy` pool in the future.

I've added one or two additional unit tests to check that `legacy` options still work with the `sequenced` pool, but haven't done anything more comprehensive than that because the future PR to ~~deprecate~~ remove the `legacy` pool will refactor all of the existing tests to use `sequenced` anyway.

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/6211
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 11:55:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6273" class=".btn">#6273</a>
            </td>
            <td>
                <b>
                    log bootnodes and static nodes list at debug level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span>
            </td>
            <td>
                at startup, log the counts (at info) and list (at debug level) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 01:00:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6268" class=".btn">#6268</a>
            </td>
            <td>
                <b>
                    Txparse subcommand implementation
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
Subcommand implementation of txparse conforming to the spec defined by @holiman [txparse impl](https://github.com/holiman/txparse/tree/main/cmd/txparse)

example usage specifying a corpus file:
```
./build/install/besu/bin/besu txparse --corpus-file=../ethereum/txparse/cmd/txparse/random_corpus.txt
```
or reading transaction lines via stdin:
```
cat ../ethereum/txparse/cmd/txparse/random_corpus.txt |./build/install/besu/bin/besu txparse
```

supersedes [besu-txparse](https://github.com/garyschulte/besu-txparse)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-09 02:21:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6267" class=".btn">#6267</a>
            </td>
            <td>
                <b>
                    ETC mainnet 'Spiral' activation block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR sets ETC Mainnet activation block as defined in [ECIP-1109](https://ecips.ethereumclassic.org/ECIPs/ecip-1109) to `19_250_000`. This change was already merged in core-geth in https://github.com/etclabscore/core-geth/pull/595
I also set the DNS discovery tree to what's in [core-geth#bootnodes_classic.go](https://github.com/etclabscore/core-geth/blob/v1.12.17/params/bootnodes_classic.go#L28)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-08 20:12:30 +0000 UTC
    </div>
</div>

