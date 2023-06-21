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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5619" class=".btn">#5619</a>
            </td>
            <td>
                <b>
                    Reload flat db strategy on clear
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

During the snapsync we can have a nullpointer because of a clear we are doing when we are starting from scratch

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 08:56:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5618" class=".btn">#5618</a>
            </td>
            <td>
                <b>
                    [4844] Check params earlier and move blob validation to a new method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Check the params earlier and move blob validation to a new method

In case CL sends a payload with invalid blob params for a known header, we should return invalid. 

Expected Behaviour: return invalid

Actual Behaviour: Returns are valid because we have already seen that payload.

This PR moves the validation earlier in the flow and encapsulates the validation login into a method for readability. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 04:13:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5613" class=".btn">#5613</a>
            </td>
            <td>
                <b>
                    services - migrate to junit 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #5558 
fixes #5557
Also pulled in some plugins tests, that extended testutil AbstractKeyValueStorageTest
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 10:17:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5612" class=".btn">#5612</a>
            </td>
            <td>
                <b>
                    Add lock to creation of pending transaction stream
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR does 2 things:

1. Takes a lock on `pendingTransactions` when creating a stream of the transactions
2. Creates a copy of the current transactions when creating the stream, rather than streaming the original list

I have tested the changes with a cut down version `PendingTransactionsForSender` class. There are a couple of points to note for the PR reviewer:

1. I don't know this area of the code well enough to know if there is likely to be a noticeable performance impact of this change. However, without it (or some alternative fix) we'll continue to see `ConcurrentModificationException` be thrown.
2. `List.copyOf` will throw a `ConcurrentModificationException` if the underlying list is changed during the call. Currently `PendingTransactionsForSender.getPendingTransactions(...)` uses that call as well, but without taking a lock on the list. I think this call could fail in the same way and I'm happy to make that change in this PR but would appreciate feedback from the reviewer first.
3. The code path that hit the issue was ultimately down to `AbstractPendingTransactionsSorter.signalInvalidAndRemoveDependentTransactions` being called which wasn't expected for the test I was running. However, the reason for the transaction and its dependent transactions being considered invalid is only logged out if trace is enabled. I wonder if this happens so often that logging it out as a `debug` message instead would be too noisy?

## Fixed Issue(s)
fixes https://github.com/hyperledger/besu/issues/5597
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 09:07:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5611" class=".btn">#5611</a>
            </td>
            <td>
                <b>
                    [4844] Ensure that blobs, proofs and  commitments have the same number of elements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">4844</span>
            </td>
            <td>
                ## PR description
Ensure blobs proofs commitments have the same size

## Fixed Issue(s)
fixes #5488 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 05:51:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5610" class=".btn">#5610</a>
            </td>
            <td>
                <b>
                    [4844] Add toString to VersionedHash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">4844</span>
            </td>
            <td>
                ## PR description
Add toString to VersionedHash and set it to be the JsonValue of the VersionedHash object

Actual: 
```
{
...
  blobVersionedHashes: [{
      versionId: 1
  }, {
      versionId: 1
  }, {
      versionId: 1
  }, {
      versionId: 1
  }, {
      versionId: 1
  }, {
      versionId: 1
  }],
 ...
}
```
Expected:

```
{
...
  blobVersionedHashes: ["0x01a8a4a49dcd1b91c376c87d7d6a6e73ee3792205864bf61781e8e3ad19d0092", 
"0x01069693395fb9a698b257e6c25380f32393bc0cf17a290f9e7fcea3c4ae7b8b", 
"0x01111dafbfcc0caa0803fc22f697fd3b9171252504e14ec0443f04a2b3288715", 
"0x01d1dfff9c15b3201980d8f9b958a8ade73e3e1e0ca76c54785a33e09519be7a", 
"0x01a7b4b55dd68d59685abcd629708c5de44c8e9edf3671602538eba23375893c", 
"0x013586020d67ab6808e681c2e6a2d1e854c84e5bc49df2ed34e218eace844f8b"],
...
}
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 03:58:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5609" class=".btn">#5609</a>
            </td>
            <td>
                <b>
                    Prepare for version 23.4.3-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 23.4.3-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 01:31:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5608" class=".btn">#5608</a>
            </td>
            <td>
                <b>
                    Release 23.4.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.4.2
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 01:00:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5607" class=".btn">#5607</a>
            </td>
            <td>
                <b>
                    Removed GoQuorum permissioning interop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Removed GoQuorum permissioning from Besu

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/5459
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-15 16:55:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5606" class=".btn">#5606</a>
            </td>
            <td>
                <b>
                    Option to disable txpool
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
        Created At 2023-06-15 15:25:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5603" class=".btn">#5603</a>
            </td>
            <td>
                <b>
                    [4844] Increase blob sidecar size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">4844</span>
            </td>
            <td>
                Increase blob sidecar size
## PR description

## Fixed Issue(s)
fixes #5590 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-15 05:02:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5601" class=".btn">#5601</a>
            </td>
            <td>
                <b>
                    [MINOR] Move noisy Pipeline log to debug
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
        Created At 2023-06-14 22:30:28 +0000 UTC
    </div>
</div>

