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
                PR <a href="https://github.com/hyperledger/besu/pull/4078" class=".btn">#4078</a>
            </td>
            <td>
                <b>
                    Fix transition protocol schedule
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
        Created At 2022-07-08 17:15:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4077" class=".btn">#4077</a>
            </td>
            <td>
                <b>
                    Release 22.4.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.4.4

cherry picks from main:
49e4fd860 -> worldstate not avail (#4069)
6aa88129e -> stateroot mismatch (#4041)
043191a40 -> jwt auth on websockets (#4039)
90f891b78 -> do not move head on exec and propose (#4013)
b5fa62c0b -> sync check before processing remote transactions (4035)
3baa4da99 -> upgrade for websockets (#4019)
5024c0788 -> sepolia TTD (#4024)
5ee9be837 -> heal step in snap (#3920)
261b1e03f -> remove peer block height requirements (#3911)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 15:32:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4075" class=".btn">#4075</a>
            </td>
            <td>
                <b>
                    Otel take 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fixes the OpenTelemetry configuration so it doesn't initialize the global opentelemetry singleton when getting the tracer.

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 11:38:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4073" class=".btn">#4073</a>
            </td>
            <td>
                <b>
                    no need to register peers connect/disconnect for Snap as well
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

SnapProtocolManager uses EthPeers so no need to handle connect/disconnect events here as well.
Eliminates some duplicated peer-related logging.

I have tested that Snap Sync works with this change

Before this change
```

2022-07-08 09:51:47.899+10:00 | nioEventLoopGroup-3-10 | TRACE | EthProtocolManager | Process message eth/66, 0
2022-07-08 09:51:47.899+10:00 | nioEventLoopGroup-3-10 | DEBUG | EthProtocolManager | Peer 0xd094aaee3baa666249... PeerReputation 100, validated? true, disconnected? false has mismatched network id: 128
2022-07-08 09:51:47.900+10:00 | nioEventLoopGroup-3-10 | TRACE | EthPeer | handleDisconnect - peer... 0xd094aaee3baa666249, PeerReputation 100
2022-07-08 09:51:47.900+10:00 | nioEventLoopGroup-3-10 | DEBUG | EthProtocolManager | Disconnect - Outbound - 0x10 SUBPROTOCOL_TRIGGERED - PeerInfo{version=5, clientId='Geth/v1.2.0-stable-9077473c/linux-amd64/go1.16.5', capabilities=[eth/65, eth/66, snap/1],
 port=0, nodeId=0xd094aaee3baa6662498e8924e26c60557b27e216ce839622fc2c123a8ea9307e4bb5a1beb108288bddeb4f04167bdcce078e89e315a4b66d0b07718fdb7930f7} - 4 peers left
2022-07-08 09:51:47.900+10:00 | nioEventLoopGroup-3-10 | DEBUG | SnapProtocolManager | Disconnect - Outbound - 0x10 SUBPROTOCOL_TRIGGERED - PeerInfo{version=5, clientId='Geth/v1.2.0-stable-9077473c/linux-amd64/go1.16.5', capabilities=[eth/65, eth/66, snap/1], port=0, nodeId=0xd094aaee3baa6662498e8924e26c60557b27e216ce839622fc2c123a8ea9307e4bb5a1beb108288bddeb4f04167bdcce078e89e315a4b66d0b07718fdb7930f7} - 4 peers left
```

After this change
```

2022-07-08 11:13:00.784+10:00 | nioEventLoopGroup-3-8 | TRACE | EthProtocolManager | Process message eth/66, 0
2022-07-08 11:13:00.784+10:00 | nioEventLoopGroup-3-8 | DEBUG | EthProtocolManager | Peer 0xbfef556cec5aa40b3e... PeerReputation 100, validated? true, disconnected? false has mismatched network id: 128
2022-07-08 11:13:00.784+10:00 | nioEventLoopGroup-3-8 | TRACE | EthPeer | handleDisconnect - peer... 0xbfef556cec5aa40b3e, PeerReputation 100
2022-07-08 11:13:00.784+10:00 | nioEventLoopGroup-3-8 | DEBUG | EthProtocolManager | Disconnect - Outbound - 0x10 SUBPROTOCOL_TRIGGERED - PeerInfo{version=5, clientId='Geth/v1.2.0-stable-d31813dc/linux-amd64/go1.16.5', capabilities=[eth/65, eth/66, snap/1],
port=0, nodeId=0xbfef556cec5aa40b3e02dd70afcac437e1689d31caaecbf68c3401f83ac9a86784c59443ff63e6e358ae7ac236f9726a620b94ba9676b899f97cb0e84a4ebcf0} - 3 peers left
```

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 05:59:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4072" class=".btn">#4072</a>
            </td>
            <td>
                <b>
                    Loads uncached logs on cache miss.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

On a miss of the on-disk logs bloom cache, we check the uncached storage, and return that if available.

## Fixed Issue(s)
fixes #3921 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 00:13:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4069" class=".btn">#4069</a>
            </td>
            <td>
                <b>
                    fix issue because parent world state is not available
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

We have this issue because we are replacing valid trielog by invalid trielog during a reorg. 

Can explain this strange trie log layer

>  : 0xd77f7f8868f20835fdfc8c7e851f6f23ce9f651d
   - StateTrieAccountValue{nonce=859, balance=0x00000000000000000000000000000000000000000000000006d141b0befb39fe, storageRoot=0x56e81f171bcc55a6ff8345e692c0f86e5b48e01b996cadc001622fb5e363b421, codeHash=0xc5d2460186f7233c927e7db2dcc703c0e500b653ca82273b7bfad8045d85a470}
   + StateTrieAccountValue{nonce=858, balance=0x00000000000000000000000000000000000000000000000006e96a274881e7b6, storageRoot=0x56e81f171bcc55a6ff8345e692c0f86e5b48e01b996cadc001622fb5e363b421, codeHash=0xc5d2460186f7233c927e7db2dcc703c0e500b653ca82273b7bfad8045d85a470}

The nonce comes from 859 to 858 and it’s not possible in a normal use case. 


### How to reproduce it (it's an example)

- We import block 5. we create a trie log for this block (4->5). A trie log it’s a diff between the previous block and the last one
- We import block 6 bis. we create a trie log for this block (5->6bis)
- We import block 7 bis. we create a trie log for this block (6bis->7bis)
- We detect a reorg with 6third with a common ancestor == 4. Rollback to 4 and we persist block 4. But in this issue we replace the valid trie log layer (3-4) with an invalid trie log (7bis->4)
- We import block 5 third. we create a trie log for this block (5 third ->6 third)
- We import block 6 third. we create a trie log for this block (6 third ->7 third)
- We detect a reorg with 6 with a common ancestor == 3. Rollback to 3 is failing because of the trie log == (7bis->4). 


In the code the problem is here

We persist after a rollback/rollfoward https://github.com/hyperledger/besu/blob/main/ethereum/core/src/main/java/org/hyperledger/besu/ethereum/bonsai/BonsaiWorldStateArchive.java#L247

We replace the trie log 
https://github.com/hyperledger/besu/blob/e79cf0e50724d7b5203708bf6b7abc24524f3dcb/ethereum/core/src/main/java/org/hyperledger/besu/ethereum/bonsai/BonsaiPersistedWorldState.java#L257


⚠️ if we have this issue we need to resync besu . there is not way to recover

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #4068 
fixes #4052

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 09:14:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4066" class=".btn">#4066</a>
            </td>
            <td>
                <b>
                    After merge add a rule to check that the current block is more recent than its parent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

In PoS current block timestamp must be greather than its parent block timestamp, so adding a new header validation rule to check that.
There is also a fix in the `shouldUsePostMergeRules` that was not correctly checking for TD >= TTD.

With this the Hive test *Invalid Ancestor Chain Re-Org, Invalid Timestamp, Invalid P9', Reveal using sync* passes.

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
        Created At 2022-07-06 18:31:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4065" class=".btn">#4065</a>
            </td>
            <td>
                <b>
                    Update dev genesis for anvil
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds anvil test accounts and milestone blocks to dev genesis. Builds on (fixing tests for) https://github.com/hyperledger/besu/pull/3872

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 11:22:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4064" class=".btn">#4064</a>
            </td>
            <td>
                <b>
                    CHANGELOG added 22.7.0-RC1 download links
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Added download links for 22.7.0-RC1

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 05:21:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4063" class=".btn">#4063</a>
            </td>
            <td>
                <b>
                    22.7.0-RC2-snapshot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

22.7.0-RC2

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 04:17:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4062" class=".btn">#4062</a>
            </td>
            <td>
                <b>
                    22.7.0-RC1 non-snapshot version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

new RC1

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 03:51:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4059" class=".btn">#4059</a>
            </td>
            <td>
                <b>
                    Log message when path unavailable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replaces https://github.com/hyperledger/besu/pull/3989

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 22:13:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4058" class=".btn">#4058</a>
            </td>
            <td>
                <b>
                    3943 stop blocks on finalized
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixed #3943 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 17:32:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4056" class=".btn">#4056</a>
            </td>
            <td>
                <b>
                    Return the correct latest valid hash in case of bad block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

In case a bad block is passed to `newPayload` or `forkchoiceUpdate` then response must contain the hash of the lastest valid block on the chain of the bad block, while now we just return the zero hash.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #3893 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 12:22:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4055" class=".btn">#4055</a>
            </td>
            <td>
                <b>
                    fcU: Ignore newHead if it is an ancestor of chain head
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description
A forkchoice update will be ignored if `newHead` is an ancestor of chain head.

## Fixed Issue(s)
fixes #4051

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 09:39:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4049" class=".btn">#4049</a>
            </td>
            <td>
                <b>
                    log for bonsai
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
        Created At 2022-07-04 09:25:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4045" class=".btn">#4045</a>
            </td>
            <td>
                <b>
                    Fix for TransitionProtocolSchedule by header when terminal block exactly at TTD
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
hive engine test "Sync Client Post Merge" highlighted a corner case with a method in TransitionProtocolSchedule which supported backward sync below/around TTD block.  

`getByBlockHeader` defers to the block header to find the appropriate pre or post merge protocol schedule, but in the case where we do not have a finalized block, and the terminal block difficulty was *exactly* the TTD value, we would erroneously return a pre-merge protocol schedule for blocks which were children of the terminal block.

PR fixes this behavior, adds some additional logging, and fixes the hive engine test.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
relates to #3841

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-02 15:10:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4044" class=".btn">#4044</a>
            </td>
            <td>
                <b>
                    add additional engine info logging 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
add info logging on engine api endpoints to increase the visibility of the EL/CL interactions

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
        Created At 2022-07-02 14:08:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4042" class=".btn">#4042</a>
            </td>
            <td>
                <b>
                    Hive engine suite conformance: Invalid Timestamp, Invalid Transition Payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Addresses failures of hive engine test suite "Invalid Timestamp" and "Invalid Transition Payload" tests.  

* on invalid timestamp, return a success response with an INVALID status and validation error message rather than error response
* for latest valid ancestor blocks which are PoW, return Hash.ZERO rather than the PoW hash 
* check tracked bad blocks for forkchoiceUpdated head blockhash, return INVALID rather than SYNCING


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
        Created At 2022-07-01 23:27:49 +0000 UTC
    </div>
</div>

