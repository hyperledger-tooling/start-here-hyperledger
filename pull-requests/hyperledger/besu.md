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
                PR <a href="https://github.com/hyperledger/besu/pull/6493" class=".btn">#6493</a>
            </td>
            <td>
                <b>
                    add profile info to help footer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #6430 

depends on #6449

![Screenshot 2024-01-30 at 3 21 48 pm](https://github.com/hyperledger/besu/assets/2627919/81aef27d-340e-4bb4-8207-20788071812d)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 05:20:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6491" class=".btn">#6491</a>
            </td>
            <td>
                <b>
                    Remove `--engine-jwt-enabled` deprecated option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Removes `--engine-jwt-enabled`. Replaced by `--engine-jwt-disabled`

It has been deprecated since 2022. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 00:45:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6490" class=".btn">#6490</a>
            </td>
            <td>
                <b>
                    [Refactor ] Move permission options to its own class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Move permission options to its own class

## Fixed Issue(s)
see #6428
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 00:29:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6487" class=".btn">#6487</a>
            </td>
            <td>
                <b>
                    Delete development artifacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Delete three files that appear to be work in progress development files.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 17:41:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6485" class=".btn">#6485</a>
            </td>
            <td>
                <b>
                    standardize on length of truncated peer ID logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span>
            </td>
            <td>
                standardise format/length of peerId in logs when not logging the entire ID / enode

fixes #6447 

After:

```
2024-01-29 17:14:44.862+10:00 | nioEventLoopGroup-3-8 | DEBUG | EthPeers | Disconnected EthPeer 0x1e853e7e7504fa3c...
2024-01-29 17:14:44.866+10:00 | nioEventLoopGroup-3-8 | DEBUG | AbstractPeerConnection | Disconnecting connection 1560687188, peer 0x1e853e7e7504fa3c... reason 0x10 SUBPROTOCOL_TRIGGERED
2024-01-29 17:14:44.867+10:00 | nioEventLoopGroup-3-2 | DEBUG | EthProtocolManager | Mismatched network id: 56, peer 0x9ad19e13619c6b50...
2024-01-29 17:14:44.869+10:00 | nioEventLoopGroup-3-2 | DEBUG | EthPeers | Disconnected EthPeer 0x9ad19e13619c6b50...
2024-01-29 17:14:44.872+10:00 | nioEventLoopGroup-3-2 | DEBUG | AbstractPeerConnection | Disconnecting connection 1737436934, peer 0x9ad19e13619c6b50... reason 0x10 SUBPROTOCOL_TRIGGERED
2024-01-29 17:14:44.874+10:00 | nioEventLoopGroup-3-7 | DEBUG | EthProtocolManager | Mismatched network id: 56, peer 0x38e30931276e4cda...
2024-01-29 17:14:44.876+10:00 | nioEventLoopGroup-3-7 | DEBUG | EthPeers | Disconnected EthPeer 0x38e30931276e4cda...
2024-01-29 17:14:44.879+10:00 | nioEventLoopGroup-3-7 | DEBUG | AbstractPeerConnection | Disconnecting connection 815991447, peer 0x38e30931276e4cda... reason 0x10 SUBPROTOCOL_TRIGGERED
2024-01-29 17:14:44.905+10:00 | nioEventLoopGroup-3-7 | DEBUG | EthProtocolManager | Mismatched network id: 56, peer 0x42b46ae6443b055d...
2024-01-29 17:14:44.905+10:00 | nioEventLoopGroup-3-5 | DEBUG | EthProtocolManager | Mismatched network id: 56, peer 0x7592f6686dcc0309...
2024-01-29 17:14:44.907+10:00 | nioEventLoopGroup-3-7 | DEBUG | EthPeers | Disconnected EthPeer 0x42b46ae6443b055d...
2024-01-29 17:14:44.907+10:00 | nioEventLoopGroup-3-5 | DEBUG | EthPeers | Disconnected EthPeer 0x7592f6686dcc0309...
2024-01-29 17:14:44.908+10:00 | nioEventLoopGroup-3-7 | DEBUG | AbstractPeerConnection | Disconnecting connection -2139568981, peer 0x42b46ae6443b055d... reason 0x10 SUBPROTOCOL_TRIGGERED
2024-01-29 17:14:44.909+10:00 | nioEventLoopGroup-3-5 | DEBUG | AbstractPeerConnection | Disconnecting connection 469943790, peer 0x7592f6686dcc0309... reason 0x10 SUBPROTOCOL_TRIGGERED
2024-01-29 17:14:44.946+10:00 | nioEventLoopGroup-3-1 | DEBUG | EthProtocolManager | Mismatched network id: 369, peer 0x315e23e64a99f688...
2024-01-29 17:14:44.947+10:00 | nioEventLoopGroup-3-3 | DEBUG | EthPeers | Disconnected EthPeer 0x3b627d2f1d0dcec9...
2024-01-29 17:14:44.952+10:00 | nioEventLoopGroup-3-1 | DEBUG | EthPeers | Disconnected EthPeer 0x315e23e64a99f688...
2024-01-29 17:14:44.955+10:00 | nioEventLoopGroup-3-1 | DEBUG | AbstractPeerConnection | Disconnecting connection -1490407832, peer 0x315e23e64a99f688... reason 0x10 SUBPROTOCOL_TRIGGERED
2024-01-29 17:14:44.989+10:00 | nioEventLoopGroup-3-9 | DEBUG | DeFramer | Peer enode://6a5b462b8a5b085bb8f791262e46bfc99208b5ec61ae7173eedfbd22f836700b34b68be0ba44243527b609cbfa1507146c77ad8f4cbab3fadf80b04851999379@1.2.3.4:30311 disconnected before sending HELLO.  Reason: 0x04 TOO_MANY_PEERS
2024-01-29 17:14:44.990+10:00 | nioEventLoopGroup-3-9 | DEBUG | RlpxAgent | Failed to connect to peer 0x6a5b462b8a5b085bb8f791262e46bfc99208b5ec61ae7173eedfbd22f836700b34b68be0ba44243527b609cbfa1507146c77ad8f4cbab3fadf80b04851999379: org.hyperledger.besu.ethereum.p2p.network.exceptions.PeerDisconnectedException: Peer disconnected for reason: 0x04 TOO_MANY_PEERS
2024-01-29 17:14:45.246+10:00 | nioEventLoopGroup-3-8 | DEBUG | EthProtocolManager | Mismatched network id: 369, peer 0x67dd6cc1cfdd993b...
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 07:19:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6484" class=".btn">#6484</a>
            </td>
            <td>
                <b>
                    Add segmented transaction get method
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
Add segmented transaction get method. This is needed to fully implement the reference counting for code storage changes to move to hashing by code hash.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 06:40:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6483" class=".btn">#6483</a>
            </td>
            <td>
                <b>
                    Report estimated disk space freed up by x-trie-log prune subcommand
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                > Prune ran successfully. We estimate you freed up 8 GiB! 🚀

Also add `--Xbonsai-trie-log-pruning-enabled` alias back in since users have started using this already
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 06:21:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6482" class=".btn">#6482</a>
            </td>
            <td>
                <b>
                    Backward Sync, reduce retries from 20 to 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
The backward sync uses the RetryingGetBlockFromPeersTask, which will try to get the block from each of the current peers. 
Only if none of the current peers can provide that block we need to retry.
If for any reason we are trying to get a block that is no longer available (reorg) we would try each of out current peers 20 times, each of our peers responding with an empty response. On an EthPeer that is responding with an empty response we will call `recordUselessResponse()`  and if we have accumulated 5 useless responses for a peer within a minute we will disconnect it.
To make sure that we do not disconnect all of our current peers this PR reduces the retries for requesting that block to 2.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 04:25:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6481" class=".btn">#6481</a>
            </td>
            <td>
                <b>
                    Fix typos
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

Fix typos in comments.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 03:56:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6480" class=".btn">#6480</a>
            </td>
            <td>
                <b>
                    remove repeated part of toString()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Remove repeated field in toString()
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 01:54:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6479" class=".btn">#6479</a>
            </td>
            <td>
                <b>
                    add sync condition for privacy tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">privacy</span><span class="chip">testing</span>
            </td>
            <td>
                addresses flakiness of privacy ATs since #6302 

fixes #6402 


cherry-picked from #5968 - kudos to @gtebrean 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 01:45:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6478" class=".btn">#6478</a>
            </td>
            <td>
                <b>
                    [Refactor] - Extract JsonRpcHttpOptions to a new class 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description


[Refactor] - Extract JsonRpcHttpOptions to a new class

Moves the JsonRpcHttpOptions cli options to its own class.
same for related tests

see #6428 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 01:30:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6477" class=".btn">#6477</a>
            </td>
            <td>
                <b>
                    [CHANGELOG] updated download links and added contributor thanks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                updated download links/shas to match https://github.com/hyperledger/besu/releases/tag/24.1.1

including errata section

Also added links for non-maintainer contributors to the latest release
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 01:10:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6474" class=".btn">#6474</a>
            </td>
            <td>
                <b>
                    filter empty ipv4 and ipv6 ping packet source addresses
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
add empty source addresses to ping packet filter lsit

currently on main we are seeing packet errors like:
```
2024-01-27 07:21:53.144+00:00 | vert.x-eventloop-thread-1 | WARN  | VertxPeerDiscoveryAgent | Sending to peer DiscoveryPeer{status=bonding, enode=enode://b3af6e4685a1c54447b0510b29397c5534a66ce32224efd250e775ebd0f56c609e3f29d76fcae1893a1b437d6d383673915d9b1c60643be0e45e52acb2f2f335@[::]:28568, firstDiscovered=1706340111143, lastContacted=0, lastSeen=1706340111143} 
failed, native error code -97, packet: 0xc76f91fa10c899a6a7d270611aba4b9f931447770a3cac9722996ebae807e0d9a403e5c090ef23cec3d81b8a27db826322dd66964656ba0acc6964ee387753796cf000fdc92e10970ec4b6e3ae12f7895c6922a0c07754ce267b98b046c124da0101eb05cb847f000001829d6f829d6fd79000000000000000000000000000000000826f98826f988465b4af4d14, stacktrace: io.netty.channel.unix.Errors$NativeIoException: sendToAddress(..) failed: Address family not supported by protocol
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
related to #6224 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-27 07:34:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6473" class=".btn">#6473</a>
            </td>
            <td>
                <b>
                    Add pragueTime configuration
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

Wire through configuration for the Prague fork, including speculative PragueGasCalculator, precompiles, and genesis options.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 22:09:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6472" class=".btn">#6472</a>
            </td>
            <td>
                <b>
                    Improve flat trace generation performance
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
When testing one of the blocks that has a lot of subcalls (838 internal transactions), we noticed that most of the time was spent on hasRevertInSubCall method. 

<img width="1720" alt="image" src="https://github.com/hyperledger/besu/assets/5099602/cac6288d-35b4-4a3c-a646-6855550b142f">

This PR reduced the time to trace a 29 mgas block from more than 5 seconds to 1 second.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 16:53:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6470" class=".btn">#6470</a>
            </td>
            <td>
                <b>
                    Write a DEBUG log entry to make it clear of a BFT node is a validator…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Currently there is nothing specifically recorded in `INFO` or `DEBUG` logs to indicate if a node is currently a validator. This PR adds a `DEBUG` log which will be produced once per block if debug logging is enabled.

## Fixed Issue(s)
No issue for this PR
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 13:43:04 +0000 UTC
    </div>
</div>

