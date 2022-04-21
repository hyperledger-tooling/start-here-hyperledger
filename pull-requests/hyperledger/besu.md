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
                PR <a href="https://github.com/hyperledger/besu/pull/3748" class=".btn">#3748</a>
            </td>
            <td>
                <b>
                    use paris evm config in merge protocolschedule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                catch exception on block persist so that it can be added to badBlocks

Signed-off-by: garyschulte <garyschulte@gmail.com>

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
        Created At 2022-04-21 18:09:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3747" class=".btn">#3747</a>
            </td>
            <td>
                <b>
                    Treat the nonce as unsigned long
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

We have to use a 64 bit value for nonce in order to be compliant with the Ethereum specifiaction. Currently we use `long` which is 64 bit, but normally only 63 bit are used for the value and one bit is used to indicate if the number is positive or negative. Which means that our nonce currently is only 63 bit long.

There are alternative functions that allow to treat `long` as a 64 bit unsigned integer, by simply interpreting all of the 64 bits as value. This PR intends to do that in order to avoid creating instances of classes like `UInt64` whenever we operate with the nonce.

## Fixed Issue(s)
Example: fixes #3702 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 06:59:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3745" class=".btn">#3745</a>
            </td>
            <td>
                <b>
                    Log full peers list on connect/disconnect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Log full list of Rlpx Connections and EthPeers (at TRACE level) on peer connect/disconnect (also added rudimentary "score" to PeerReputation - not used anywhere as yet) eg
```
2022-04-21 12:21:27.470+10:00 | pool-8-thread-1 | TRACE | RlpxAgent | 2 ConnectionsById {
LocallyInitiatedRlpxConnection initiatedAt:1650507687470 to 0x3548c87b9920ff16aa4bdcf01c85f25117a29ae1574d759bad48cc9463d8e9f7c3c1d1e9fb0d28e73898951f90e02714abb770fd6d22e90371882a45658800e9 disconnected? false,
LocallyInitiatedRlpxConnection initiatedAt:1650507687469 to 0xdcb9390953aec5dde1d60dd556c36827053ca9adaefd1b03f531592fea43824bae2919743f620bb8a9b6c2b9a54439771d4f9a74d261b74af7a10c2dd9f13c97 disconnected? false} 
```
and ethPeers (different example - note 2 peers with same enode, one is "disconnected")
```
2022-04-21 11:17:23.192+10:00 | nioEventLoopGroup-3-2 | TRACE | EthProtocolManager | 2 EthPeers {
Peer 0xdcb9390953aec5dde1... PeerReputation 100, validated? true, disconnected? false, 
Peer 0xdcb9390953aec5dde1... PeerReputation 100, validated? true, disconnected? true} 
```
See #3665 

Also log peer reputation on disconnect See #3666 eg
```
2022-04-21 13:01:33.990+10:00 | nioEventLoopGroup-3-2 | TRACE | EthPeer | handleDisconnect - peer... 0x3548c87b9920ff16aa, PeerReputation 100 
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
        Created At 2022-04-21 01:37:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3741" class=".btn">#3741</a>
            </td>
            <td>
                <b>
                    Use pivot header download time to select sync target
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
We previously select the peer with the best chain when selecting a sync target - this makes little sense and this PR uses the pivot block header download time as the comparator instead.

## Fixed Issue(s)
#3736 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 05:24:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3737" class=".btn">#3737</a>
            </td>
            <td>
                <b>
                    test block import
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
        Created At 2022-04-19 10:22:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3734" class=".btn">#3734</a>
            </td>
            <td>
                <b>
                    Thread safe rocksdb segment handles
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

Ensure thread-safe access to rocksdb column family segments, in case we have dropped and recreated a columnFamily in `RocksDBColumnarKeyValueStorage.clear()`.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3722


## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 20:27:08 +0000 UTC
    </div>
</div>

