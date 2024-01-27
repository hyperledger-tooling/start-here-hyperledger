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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6468" class=".btn">#6468</a>
            </td>
            <td>
                <b>
                    Fix 24.1.1 changelog
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
fix changelog:
 * 24.1.1 entries 
 * 24.1.0 download links
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 01:01:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6466" class=".btn">#6466</a>
            </td>
            <td>
                <b>
                    Log blob count when importing a block via Engine API
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

Log blob count when importing a block via engine API, plus removing an unused method leftover from a previous cleanup

Log lines look like these:
```
{"@timestamp":"2024-01-25T11:21:32,538","level":"INFO","thread":"vert.x-worker-thread-0","class":"AbstractEngineNewPayload","message":"Imported #10,431,117 / 44 tx / 16 ws / 3 blobs / base fee 11 wei / 4,868,888 (16.2%) gas / (0x79916291a34d7075190b88872c06ee9e89b5350fd04e57b0430c2a6da3620a45) in 0.874s. Peers: 1","throwable":""}
{"@timestamp":"2024-01-25T11:21:33,571","level":"INFO","thread":"vert.x-worker-thread-0","class":"AbstractEngineNewPayload","message":"Imported #10,431,118 / 47 tx / 16 ws / 1 blobs / base fee 11 wei / 8,522,787 (28.4%) gas / (0xec4f4f0f87d4df8bbac2f07a810f46dbb2c7eccef0ae67c3a15aa7ca145d7b25) in 0.904s. Peers: 1","throwable":""}
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-25 11:25:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6463" class=".btn">#6463</a>
            </td>
            <td>
                <b>
                    Skip pruning if trie log count is less than retention limit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Rework error messaging in this case.

This can occur if pruning is attempted before the node has reached the configured retention limit (512 by default)

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
        Created At 2024-01-25 03:15:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6461" class=".btn">#6461</a>
            </td>
            <td>
                <b>
                    [Refactor] - Extract websocket options to a new class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
[Refactor] - Extract web socket options to a new class

- Moves the web socket cli options to its own class.
- same for related tests

## Fixed Issue(s)
see #6428
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-25 01:59:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6460" class=".btn">#6460</a>
            </td>
            <td>
                <b>
                    Release 24.1.1
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
release version of 24.1.1 including:
 - 24.1.1-RC commits
 - RC2 cherry picks of:
   - #6455 
   - #6458
 - updated changelog

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-24 22:10:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6459" class=".btn">#6459</a>
            </td>
            <td>
                <b>
                    info level log for pipeline abort
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

Draft PR just to get a deployable artifact 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-24 21:50:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6458" class=".btn">#6458</a>
            </td>
            <td>
                <b>
                    silence dns query error warning
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
Temporary measure to silence the DNS query WARN errors until we can get an upstream library change in tuweni-dns-discovery

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #6070 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-24 18:11:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6456" class=".btn">#6456</a>
            </td>
            <td>
                <b>
                    Add broadcast address to PingPacketData from filter
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
address another pathological default PingPacketData from address we are seeing on mainnet - a broadcast address 255.255.255.255 seems to be a default value for some implementations.

For example we are seeing a lot of these log lines on mainnet:
```
{
   "@timestamp":"2024-01-24T06:18:16,129",
   "level":"WARN",
   "thread":"vert.x-eventloop-thread-3",
   "class":"VertxPeerDiscoveryAgent",
   "message":"Sending to peer DiscoveryPeer{status=bonding, enode=enode://5d01e72875f3485fdcce5255720696087ea7d704c6632282fbe39329db6417a6f5ef940cf05519677be7f9c31b6b553fe9192e9e9feed37db3fb97bcc7fd099e@255.255.255.255:30313, firstDiscovered=1706077069751, lastContacted=0, lastSeen=1706077069751} failed, native error code -13, packet: 0x3123aed37feabe25bd4cc2625a1d1e2b12a5a1bbe6f3ef594c1ea76abbfbae670ab30477655186a5a3bf4487f2fa183807dad26037e950e89cc07ba20eaf229437e69c2e56d44fe934082147098ca4a0bd99964d67d2046789d080f69d5be2c60101df05cb8489757c7882765f82765fcb84ffffffff8276698276698465b0abe402, stacktrace: io.netty.channel.unix.Errors$NativeIoException: sendToAddress(..) failed: Permission denied",
   "throwable":""
}
```

the functional change is minimal, but rearranges the host detection to be in a unit testable method.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
related to #6224 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-24 15:45:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6455" class=".btn">#6455</a>
            </td>
            <td>
                <b>
                    ignore bws sync requests until initial sync is complete
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

Ensure we do not attempt to start BWS sessions if initial sync has not yet completed.  This change prevents BWS from triggering via engine-api during:
* initial sync
* auto-heal
* resync worldstate

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 23:07:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6453" class=".btn">#6453</a>
            </td>
            <td>
                <b>
                    feat: add `OperationTracer.tracePrepareTransaction`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

`OperationTracer.traceStartTransaction` is triggered before the EVM execution, but after the sender account has been updated (i.e. its balance decreased from the upfront cost and its nonce increased), hiding its actual initial state from the `OperationTracer`.

This PR adds a new hook, `OperationTracer.tracePrepareTransaction`, that is triggered after the transaction has been validated for execution, but before any change to the sender account, hence presenting its pristine state to the `OperationTracer`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 17:49:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6452" class=".btn">#6452</a>
            </td>
            <td>
                <b>
                    Feature/keccak impro
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
        Created At 2024-01-23 14:23:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6451" class=".btn">#6451</a>
            </td>
            <td>
                <b>
                    manage empty range for storage
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
        Created At 2024-01-23 14:22:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6449" class=".btn">#6449</a>
            </td>
            <td>
                <b>
                    Add minimalist staker profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Add minimalist staker profile

Use
`besu --profile=minimalist_staker`

## Fixed Issue(s)
fixes https://github.com/hyperledger/besu/issues/6324
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 04:13:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6448" class=".btn">#6448</a>
            </td>
            <td>
                <b>
                    Add enterprise/private profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add enterprise/private profile 

Use:
`besu --profile=enterprise` or `besu --profile=private`

## Fixed Issue(s)
fixes #6326
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 03:55:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6446" class=".btn">#6446</a>
            </td>
            <td>
                <b>
                    Enable limit on range Of JSON-RPC API trace_filter method (#5971)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span><span class="chip">RPC</span>
            </td>
            <td>
                Enable a limit on the range of blocks that can be supplied to the JSON-RPC trace_filter method.

The limit has a default value and can be overridden with a command line option at start up.

fixes #5971 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 21:27:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6445" class=".btn">#6445</a>
            </td>
            <td>
                <b>
                    Reuse --bonsai-historical-block-limit for limit trie logs feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Part of https://github.com/hyperledger/besu/issues/5390

* `$BESU --Xbonsai-limit-trie-logs-enabled=true` will use the default value of `--bonsai-historical-block-limit=512`
* `$BESU --Xbonsai-limit-trie-logs-enabled=true --bonsai-historical-block-limit=511` throws error as must be >= 512
* `$BESU --Xbonsai-limit-trie-logs-enabled=false --bonsai-historical-block-limit=511` does not throw error as this is allowed until limit-trie-logs-enabled.

This implementation avoids a breaking change for anyone that has a node with --bonsai-historical-block-limit already set to < 512 (could be noone?)

However, we should be aware that if `--Xbonsai-limit-trie-logs-enabled` ever becomes default then this breaking change will come back again
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 21:20:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6444" class=".btn">#6444</a>
            </td>
            <td>
                <b>
                    Fix `poa-block-txs-selection-max-time` option that was inadvertently reset to its default after being configured
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

Fix `poa-block-txs-selection-max-time` option that was inadvertently reset to its default after being configured.
Mining options needs the value of the block period from the genesis file, so the way to pass it to the class has been improved to avoid using the mining options if that value was not set, in order to be less error prone.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 14:58:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6443" class=".btn">#6443</a>
            </td>
            <td>
                <b>
                    Disconnect worst peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
In AbstractRetryingSwitchingPeerTask.java the method refreshPeers() we are now disconnecting the least useful peer. 
Another change is that now the peer table is refreshed until we have reached our maxPeers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 08:22:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6441" class=".btn">#6441</a>
            </td>
            <td>
                <b>
                    Ensure that Bonsai tests with Key Value storage are using Bonsai data configuration
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
Ensure that Bonsai tests with Key Value storage are using Bonsai data configuration. As these key-value storage are explicit with Bonsai classes this doesn't cause an issue using the default forest config but for readability, it is better to use the Bonsai data storage configuration.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 01:43:30 +0000 UTC
    </div>
</div>

