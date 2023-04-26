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
                PR <a href="https://github.com/hyperledger/besu/pull/5392" class=".btn">#5392</a>
            </td>
            <td>
                <b>
                    remove zero lead bytes of log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">performance</span><span class="chip">mainnet</span><span class="chip">TeamChupa</span><span class="chip">bonsai</span>
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
        Created At 2023-04-26 13:56:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5385" class=".btn">#5385</a>
            </td>
            <td>
                <b>
                    Permissioning - A better solution to fix NullPointerException on createPayload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This is a more elegant solution then PR 5374 for issue 5370. When running on docker, URI returns null on getHost() method but returns the correct hostname on toString() method, owning to the 'underline character' on hostname in docker-compose services.

## Fixed Issue(s)
#5370 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 21:51:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5380" class=".btn">#5380</a>
            </td>
            <td>
                <b>
                    prepare main for next point release
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
update changelog
prep for next point release

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-21 20:25:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5379" class=".btn">#5379</a>
            </td>
            <td>
                <b>
                    Prepare for version 23.4.0-RC2-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 23.4.0-RC2-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-21 20:02:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5378" class=".btn">#5378</a>
            </td>
            <td>
                <b>
                    Burn-in release 23.4.0-RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 23.4.0-RC1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-21 19:10:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5375" class=".btn">#5375</a>
            </td>
            <td>
                <b>
                    Unified protocol schedule tidy up
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Some straight forward refactorings and tidy up

- [x] Fold AbstractProtocolScheduleBuilder into ProtocolScheduleBuilder
- [x] Tidy up WithdrawalsValidatorProvider
- [x] Maybe no need to createSchedule inside JsonRpcMethodsFactory, as per https://github.com/hyperledger/besu/pull/5310#discussion_r1172086249
- [x] Unify StreamingProtocolSchedules and extend UnifiedProtocolSchedule
- [x] Rename UnifiedProtocolSchedule -> DefaultProtocolSchedule

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Part of https://github.com/hyperledger/besu/issues/5354

## Testing

- [x] local validator interop (beku-timestamp) with tx-fuzz
- [x] near head checkpoint sync sepolia
- [x] checkpoint sync sepolia
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 23:54:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5374" class=".btn">#5374</a>
            </td>
            <td>
                <b>
                    Permissioning - Fix NullPointerException on createPayload (Issue #5370)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">permissioning</span><span class="chip">non mainnet (private networks)</span>
            </td>
            <td>
                ## PR description
Tries not pass `null` value to `List.of` on method `org.hyperledger.besu.ethereum.permissioning.NodeSmartContractV2PermissioningController.createPayload`
Sometimes method `enodeUrl.toURI().getHost()` returns `null`. In this case, we use `enodeUrl.getIpAsString()` to get IP address. And, if this method returns `null`, use empty String in `List.of`.

## Fixed Issue(s)
fixes #5370


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 17:56:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5372" class=".btn">#5372</a>
            </td>
            <td>
                <b>
                    Bonsai TrieLogFactory serializer/deserializer
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
This PR introduces a TrieLogFactory interface and default implementation that will allow for a pluggable implementation of bonsai trie log serialization and deserialization.  

This pr also introduces a StorageSlotKey record type that enables accumulators and serializers to utilize slotKeys and/or slotKeyHashes when writing trieLogs.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
related to protocol-misc # 755
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 01:42:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5371" class=".btn">#5371</a>
            </td>
            <td>
                <b>
                    Retire ECIP-1049 network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
With the [withdraw](https://github.com/ethereumclassic/ECIPs/pull/486) of ECIP-1049 we can remove the network meant for testing.
This PR also removes Keccak pow/hasher but I'm good with keeping those.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 00:13:30 +0000 UTC
    </div>
</div>

