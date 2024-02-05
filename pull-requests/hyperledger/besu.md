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
                PR <a href="https://github.com/hyperledger/besu/pull/6500" class=".btn">#6500</a>
            </td>
            <td>
                <b>
                    [MINOR] remove duplicate setting of default values for CLI options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                where the default is number/boolean/string, just leave it to the initialized value for the actual field.

same as was done for Sync Options in #6499
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 01:44:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6499" class=".btn">#6499</a>
            </td>
            <td>
                <b>
                    Flat db heal - deprecate CLI option and set to always true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * set flat db healing enabled to true always
* remove duplicate setup of default values from Sync Options class

refs #6157
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 01:26:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6498" class=".btn">#6498</a>
            </td>
            <td>
                <b>
                    Filter Discovered peers for ipv6 support
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
updates PeerDiscoveryAgent to 
* use existing NetworkUtility to filter for any/none peers
* fall back to source address if ipv6 is not supported (like in a docker container)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #6475 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 01:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6496" class=".btn">#6496</a>
            </td>
            <td>
                <b>
                    [Refactor] Move graphqloptions to its own class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Move GraphQl options options to its own class

## Fixed Issue(s)
see https://github.com/hyperledger/besu/issues/6428
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 21:46:25 +0000 UTC
    </div>
</div>

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

