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
                PR <a href="https://github.com/hyperledger/besu/pull/3620" class=".btn">#3620</a>
            </td>
            <td>
                <b>
                    Use JUnit 5 for unit test execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Change the unit test execution to use the Junit5 JUnitPlatform. This
allows for a mix of junit 4 and junit 5 tests and for a gradual
migration to junit 5 instead of a big bang. One class depended on
junit 4 exceptions and was updated.

Also, this facilitated a slight refactor of TLSContextFactoryTest so 
that when running on a mac (typical developer machine) errors stemming
from the nss3 library do not cause unit test failures, while still 
testing non-nss3 code paths. Tests will perform normally in integration.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 00:33:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3617" class=".btn">#3617</a>
            </td>
            <td>
                <b>
                    Return GOQUORUM_PRIVATE_STORAGE where it was
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR should put back a missing GOQUORUM_PRIVATE_STORAGE enum that I accidentally removed.

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-21 14:51:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3616" class=".btn">#3616</a>
            </td>
            <td>
                <b>
                    Improve eth/66 support
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

Currently Besu has a limited support for sending NewPooledTransactionHashes messages, and other aspect related to reduce transactions synchronization traffic, described in the [Ethereum Wire Protocol](https://github.com/ethereum/devp2p/blob/master/caps/eth.md#ethereum-wire-protocol-eth) version 66.

Specifically:
1. Besu only uses NewPooledTransactionHashes for new local transactions, while it could be extended to any transaction added to the transaction pool
2. Besu does not limit the sending of the full transaction messages to a small fraction of the connected peers, and sends the new transaction hashes to all the remaining peers

This PR, extends eth/66 support and does some code refactoring, to remove some reduntant code and rename some classes to identify they are related to the NewPooledTransactionHashes message.

The main changes are:
1. Do not have a separate tracker for transaction hashes, since for them we can reuse PeerTransactionTracker, that tracks full transactions exchange history and sending queue with a peer. So PeerPendingTransactionTracker has been removed.
2. When a new peer connects, if it support eth/6[56] then we send all the transaction hashes we have in the pool, otherwise we send the full transactions.
3. When new transactions are added to the pool, we send full transactions to peers without eth/6[56] support, or to a small fractions of all peers, and then we send only transaction hashes to the remaining peer that support eth/6[56]. Both transactions and transaction hashes are only sent if not already exchanged with that specific peer.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-21 13:44:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3615" class=".btn">#3615</a>
            </td>
            <td>
                <b>
                    rename premerge fork to paris, keep premerge as an alias
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
rename the merge fork to `paris`
keep `premerge` as an alias for paris 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3608

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-19 14:52:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3611" class=".btn">#3611</a>
            </td>
            <td>
                <b>
                    [DO NOT MERGE] During Fast Sync execute World State Construction before Blocks Import
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Performance Test :
During Fast Sync execute World State Construction before Blocks Import

Signed-off-by: Ameziane Hamlat ameziane.hamlat@consensys.net

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 13:39:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3610" class=".btn">#3610</a>
            </td>
            <td>
                <b>
                    Tune transaction synchronization parameter to adapt to mainnet traffic
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
This PR is composed of the tuning of some internal parameters related to the transaction synchronization.

1. Currently Besu handles hundreds of transaction message per seconds, so having a queue of 1M messages result in a lot of expired messages, make sense to reduce the capacity to drop incoming messages that could not be handled anyway.
2. Currently on mainnet there are many thousand of pending transactions exchanged between peers, but Besu has a short memory of what has been exchanged with a specific peer, with the result that the same transaction is often exchanged back and forth with the same peer, expecially when the peer is another Besu (below a sample of one transaction exchanged many time between peers) so it is necessary to remember more transactions seen with peers.
3. Added detailed information about exchanged transactions at trace log level.

This is a sample extraction from the trace logs of one transactions, peers `0x0b7cbef740d1af50cf`, `0xec1e73d0839ec87abe`, `0x364c56424b81989e57` are other Besus
[tx-sample.pdf](https://github.com/hyperledger/besu/files/8303223/tx-sample.pdf)


Running this patch on a 4 Besu nodes for some hours, showns that CPU and memory usage is significantly reduced
![image](https://user-images.githubusercontent.com/91944855/159009115-a5673f15-e722-4ac3-86d2-a65c1aa68848.png)


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->


<!-- Example: "fixes #2" -->
fixes #3524 
## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 09:31:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3607" class=".btn">#3607</a>
            </td>
            <td>
                <b>
                    Bugfix/stuck at ttd
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
* fix a corner case where besu does not recognize TTD block descending from TTD
* extend the distance that besu will 'look back' for TTD block in the case of a long period on non-finality post-merge
* added MergeCoordinator.addNewPayloadToSync to append newPayload to backward sync if we short circuit newPayloads early due to missing parent hash

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3609

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 04:42:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3606" class=".btn">#3606</a>
            </td>
            <td>
                <b>
                    quorum ATs task does not depend on building docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

remove gradle dependency

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 04:25:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3604" class=".btn">#3604</a>
            </td>
            <td>
                <b>
                    [MINOR] add RPC method name to log for InvalidParams
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>
BEFORE
```
2022-03-18 13:38:22.593+10:00 | vert.x-worker-thread-0 | DEBUG | JsonRpcHttpService | Invalid Params
org.hyperledger.besu.ethereum.api.jsonrpc.internal.exception.InvalidJsonRpcParameters: Invalid json rpc parameter at index 1
Caused by: com.fasterxml.jackson.databind.exc.ValueInstantiationException: Cannot construct instance of `org.hyperledger.besu.ethereum.api.jsonrpc.internal.parameters.TraceTypeParameter`, problem: Invalid trace types supplied: foo
 at [Source: (String)"["foo","stateDiff"]"; line: 1, column: 19]
```
AFTER:
```
2022-03-18 13:38:22.593+10:00 | vert.x-worker-thread-0 | DEBUG | JsonRpcHttpService | Invalid Params for method: trace_rawTransaction
org.hyperledger.besu.ethereum.api.jsonrpc.internal.exception.InvalidJsonRpcParameters: Invalid json rpc parameter at index 1
Caused by: com.fasterxml.jackson.databind.exc.ValueInstantiationException: Cannot construct instance of `org.hyperledger.besu.ethereum.api.jsonrpc.internal.parameters.TraceTypeParameter`, problem: Invalid trace types supplied: foo
 at [Source: (String)"["foo","stateDiff"]"; line: 1, column: 19]
```

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 03:42:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3602" class=".btn">#3602</a>
            </td>
            <td>
                <b>
                    [MINOR] added toString for TraceTypeParameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

so that logging can work properly

See https://github.com/hyperledger/besu/issues/3528

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 23:33:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3601" class=".btn">#3601</a>
            </td>
            <td>
                <b>
                    SNAPSYNC add request task
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">snapsync</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

PR that adds the different request tasks necessary for the snapsync as well as a utility to manage the ranges of requests 

Snapsyc is still an experimental feature more tests will be added when the feature will be completed

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 15:54:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3595" class=".btn">#3595</a>
            </td>
            <td>
                <b>
                    added download links for 22.1.2 and moved bonsai change to 22.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Added 22.1.3 section to changelog

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 09:23:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3594" class=".btn">#3594</a>
            </td>
            <td>
                <b>
                    change snapshot version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

Change snapshot version to 21.1.3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 05:59:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3592" class=".btn">#3592</a>
            </td>
            <td>
                <b>
                    address some sonar cloud bugs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

constants for strings and check some optionals.
Also changed the engineHttpUrl() method to use the engine host 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 05:14:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3591" class=".btn">#3591</a>
            </td>
            <td>
                <b>
                    Display data storage options in CLI help
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Diego López León <dieguitoll@gmail.com>

## PR description
This is a leftover from #3578 to display the new stable options in the `--help` output
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 04:52:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3590" class=".btn">#3590</a>
            </td>
            <td>
                <b>
                    Upgrade Tuweni to version 2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update Tuweni to version 2.2. 
This updates the version of icu4j, fixing a vulnerability:
https://www.sourceclear.com/vulnerability-database/security/integer-overflow/java/sid-7705
https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2018-18928

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 04:42:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3589" class=".btn">#3589</a>
            </td>
            <td>
                <b>
                    Release 22.1.2
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
        Created At 2022-03-16 04:30:17 +0000 UTC
    </div>
</div>

