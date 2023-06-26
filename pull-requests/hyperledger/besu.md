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
                PR <a href="https://github.com/hyperledger/besu/pull/5640" class=".btn">#5640</a>
            </td>
            <td>
                <b>
                    Eth/68: treat transaction size as scalar unsigned int
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

Align Besu to what other clients are doing, treating the sizes as an array of scalar ints and not 4 bytes, this also prevent being disconnected from Geth due to `invalid-message` error:

```
DEBUG[06-19|15:15:40.347] Ethereum peer connected                  id=a1697db12e1f2986 conn=inbound name=besu/v23.4.0/linux-x...
DEBUG[06-19|15:15:40.360] Message handling failed in `eth`         id=a1697db12e1f2986 conn=inbound err="invalid message: message msg #8 (157028 bytes): invalid message: (code 8) (size 157028) rlp: non-canonical integer (leading zero bytes) for uint32, decoding into (eth.NewPooledTransactionHashesPacket68).Sizes[0]"
DEBUG[06-19|15:15:40.360] Removing p2p peer                        peercount=10 id=a1697db12e1f2986 duration=12.956ms     req=false err="invalid message: message msg #8 (157028 bytes): invalid message: (code 8) (size 157028) rlp: non-canonical integer (leading zero bytes) for uint32, decoding into (eth.NewPooledTransactionHashesPacket68).Sizes[0]"
```

Contacting the author of the EIP for making it clearer in which data type is used for this message.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 14:21:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5639" class=".btn">#5639</a>
            </td>
            <td>
                <b>
                    Update evmtool graalvm build
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

Update EVMTool's GraalVM build
* add new class to reflection config
* move CLI output to be system-err oriented
* make logger in evmtool nop
* exclude some problematic jars from compilation
  - mixed versions of bouncy castle
  - netty initializations of log4j

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-24 15:55:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5638" class=".btn">#5638</a>
            </td>
            <td>
                <b>
                    Updates for execution-spec-tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Updates needed to keep executing execution-spec-tests
* add withdrawals support
* add access lists to transactions
* accept t8n and b11r CLI args that are zero length or all whitespace
* Enumerate forks in t8n and b11r help
* remove JSON wrapping from t8n transaction RLP

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 21:23:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5637" class=".btn">#5637</a>
            </td>
            <td>
                <b>
                    Fail fast in case of downgrade done without reverting variables storage
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

#5471 is backward incompatible, and there is a procedure to do before downgrading, but if the procedure is not followed the db becomes inconsistent, to avoid that this PR tries to detect this scenario and fail fast in case it founds a previous migration, giving the user a possibility to retry the rollback procedure.

If an inconsistency is found this log is printed

```
2023-06-23 16:06:21.885+00:00 | main | ERROR | KeyValueStoragePrefixedKeyBlockchainStorage | Inconsistency found when migrating chainHeadHash to variables storage, probably this is due to a downgrade done without running the `storage revert-variables` subcommand first, see https://github.com/hyperledger/besu/pull/5471
chainHeadHash mismatch: blockchain storage value=0x25a5cc106eea7138acab33231d7160d69cb777ee0c2c553fcddf5138993e6dd9, variables storage value=0x8a3d34ff1d0c4e57fad7c5ec2e316cad84e590e38bd93c386a3ade49deb0437f
```

Tested with this scenario:
1. Existing 23.4.1 Besu with already synced db
2. Upgrade to 23.4.3 and variables migrated
3. Downgrade to 23.4.1 *without* running `storage revert-variables` first, got `World State Root does not match expected value, header 0x5eb6e371a698b8d68f665192350ffcecbbbf322916f4b51bd79bb6887da3f494 calculated 0x0ec284a94272bbfe33f8455acb8f182401607bda6b71c75c3d5584d719e7d8e7`
4. Upgrade again to 23.4.3 and then Besu correctly fails to start since inconsistency detected, with the log reported above.
5. Run `storage revert-variables` successfully rollback variables storage
6. Downgrade again to 23.4.1 and this time Besu starts correctly

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 14:21:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5635" class=".btn">#5635</a>
            </td>
            <td>
                <b>
                    Add debug_getRawTransaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add the new debug_getRawTransaction to the DEBUG engine

## Fixed Issue(s)
Part of #5377 
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 22:31:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5634" class=".btn">#5634</a>
            </td>
            <td>
                <b>
                    Start with txpool disabled
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

This PR review the way the txpool is enabled/disabled in a more intuitive way and also[ fix a bug ](https://github.com/hyperledger/besu/issues/5636)that happens when enabling the layered txpool when not synced.

The main point of disabling the txpool, is to avoid its overhead during the initial sync (or resync) phases, since pending transactions are always evaluated and processed against the current head, so if we are syncing there is no value in processing them, and we can wait until the sync is done to enabled the txpool.
The current implementation is a bit convoluted, since the txpool is always enabled at startup, but if the initial sync is not done, then the txpool is disabled, to be re-enabled after the sync is done, while it is straightforward to just start with the txpool disabled, and enabled it when the sync is done.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #5636 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 19:51:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5633" class=".btn">#5633</a>
            </td>
            <td>
                <b>
                    consensus/ibft junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                Refs #5569 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 06:51:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5632" class=".btn">#5632</a>
            </td>
            <td>
                <b>
                    consensus/merge junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                Refs #5569
Added lenient() in some spots
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 06:10:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5631" class=".btn">#5631</a>
            </td>
            <td>
                <b>
                    [MINOR] config module - junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                Fixes #5570
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 04:30:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5630" class=".btn">#5630</a>
            </td>
            <td>
                <b>
                    Faster MCOPY implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                wire in deep call to System.arrayCopy instead of buffer copy.

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
        Created At 2023-06-21 20:27:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5629" class=".btn">#5629</a>
            </td>
            <td>
                <b>
                    Decouple JsonRpcError enum from the data field
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
Moves data field from JsonRpcError enum to JsonRpcErrorResponse to avoid its reset when enum is reused.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
Fixes #5437

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 16:25:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5628" class=".btn">#5628</a>
            </td>
            <td>
                <b>
                    Make fork id the default and try to recover the DiscoveryPeer for incoming connections from the PeerTable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR introduces these changes:
- Make "--filter-on-enr-fork-id" default to true. That means that Besu by default will request the ENR from peers it has bonded with, which usually contains the fork id. The fork id then is used to find out whether that peer is on the same chain.
- When other peers are initiating a handshake with us we now will check our PeerTable to see whether we have bonded with that peer. If the peer is found in the PeerTable we can check if the fork id is available to find out whether that peer is on the same chain.

Only if the fork id indicates that the peer is on the same chain we will try to establish a connection with that peer.

## Fixed Issue(s)
#5272 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 07:01:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5627" class=".btn">#5627</a>
            </td>
            <td>
                <b>
                    [CHANGELOG] tuweni update was reverted
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix changelog.
Tuweni update was reverted #5585 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-21 00:27:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5623" class=".btn">#5623</a>
            </td>
            <td>
                <b>
                    t8n server implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description
When used as a tool for cross testing, the `evm t8s` tool shows performance issues caused by the continous JVM context load which prevents the tool to be included in the [cross testing integration suite](http://retesteth.ethdevops.io/).
This PR adds a subcommand to `evm` named `t8n-sever, which starts a HTTP server able to handle JSON request with the following structure:
```json
{
  "state": {
    "fork": ...,
    "chainid": ...,
    "reward": ...
  },
  "input": {
    "env": { ... },
    "alloc": { ... },
    "txs": [ ... ]
  }
}
```
each field matches the parameters of the `evm t8n` tool, but for when a path is expected, the full content of the file has to be passed.

This implementation was tested by @winsvega who confirmed the performance boost

### Developer considerations
 - This server doesn't need to be a subcommand. It's there just to follow the existing `t8n` _pattern_, but no `evm` option will have any effect on its behavior.
 - This type of server for `t8n` tests is also used by at least one other client, i.e. [ethereumjs](https://github.com/ethereumjs/ethereumjs-monorepo/blob/%40ethereumjs/vm%406.5.0/packages/vm/test/retesteth/transition-cluster.ts#L53), but in their case they expect the server to have access to the tests executor file system.
 - Eventually we could analyze to deprecate the existing [retesteth RPC Interface](https://ethereum-tests.readthedocs.io/en/latest/rpc-ref.html) ([reference code](https://github.com/hyperledger/besu/blob/23.4.3/besu/src/main/java/org/hyperledger/besu/cli/subcommands/RetestethSubCommand.java)) as it doesn't provide all the features required after the transtion of ETH to PoS.
 - The performance of this new server doesn't match the one that once had the mentioned RPC retesteth service.
 - This server has been tested using a modified version of [ethereum/retesteth](https://github.com/ethereum/retesteth/)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 18:33:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5621" class=".btn">#5621</a>
            </td>
            <td>
                <b>
                    Prepare for version 23.4.4-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 23.4.4-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 03:34:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5620" class=".btn">#5620</a>
            </td>
            <td>
                <b>
                    Release 23.4.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.4.3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 03:13:03 +0000 UTC
    </div>
</div>

