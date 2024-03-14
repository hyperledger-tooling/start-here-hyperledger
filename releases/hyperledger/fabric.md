---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v3.0.0-beta
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v3.0.0-beta
                </span>
            </td>
            <td>
                v3.0.0-beta Release Notes - March 14, 2024
==========================================

The v3.0.0-beta release is an early release of Fabric v3.0, specifically to demonstrate and get feedback on the new Byzantine Fault Tolerant (BFT) ordering service.

v3.0.0-beta is not intended to be used in production and is not intended as an upgrade target from prior versions. It can however be used to test the process
for migrating from Raft to SmartBFT consensus.

New features
------------

**Byzantine Fault Tolerant (BFT) ordering service**

Hyperledger Fabric has utilized a Raft crash fault tolerant (CFT) ordering service since version v1.4.1.
A Byzantine Fault Tolerant (BFT) ordering service can withstand not only crash failures, but also a subset of nodes behaving maliciously.
Fabric v3.0.0-beta provides a BFT ordering service based on the [SmartBFT](https://arxiv.org/abs/2107.06922) [consensus library](https://github.com/SmartBFT-Go/consensus).
Consider using the BFT orderer if true decentralization is required, where up to and not including a third of the parties running the orderers may not be trusted due to malicious intent or being compromised.
For more details of the BFT ordering service and other recent features, see the [What's New documentation](https://hyperledger-fabric.readthedocs.io/en/latest/whatsnew.html).

The v3.0.0-beta release differs from the v3.0.0-preview release by making the peer and orderer block replication resistant to block withholding. 
Block withholding is when an orderer receives a request for blocks it possesses, but it delays sending the blocks and by doing so, slows down the requester's block reception.
As described in [the RFC](https://hyperledger.github.io/fabric-rfcs/text/0010-bft-signatures.html), block withholding resistance incurs a bandwidth and CPU cost,
and therefore an operator of an orderer may opt out and use the standard mechanism by specifying `ReplicationPolicy`: `simple` in the local configuration.

**Query all approved chaincodes on a channel**

The updated `peer lifecycle chaincode queryapproved` command allows you to pass only a channel name.
The command will return all approved chaincodes on the channel.


Improvements and Fixes
----------------------

All improvements and fixes as of v2.5.6 have also been included in v3.0.0-beta.


Dependencies
------------
Fabric v3.0.0-beta has been tested with the following dependencies:
* Go 1.21.8
* CouchDB v3.3.3

Fabric docker images on dockerhub utilize Ubuntu 20.04.


Changes
-------

**peer.gossip.pvtData.transientstoreMaxBlockRetention default value increased from 1000 to 20000**

`peer.gossip.pvtData.transientstoreMaxBlockRetention` specifies the number of blocks to keep uncommitted private data
in the transient store before it is purged. Increasing the value provides more tolerance for delayed commits
before the data is purged.


Removals
--------

**Support for ordering service system channel has been removed**

v2.3 introduced the ability to manage an ordering service without a system channel.
Managing an ordering service without a system channel has privacy, scalability, and operational benefits.
The system channel is removed in Fabric v3.0, as well as the concept of a 'consortium' of organizations that can create channels.
If you used the system channel in prior releases, you must remove the system channel and migrate to the channel participation API before upgrading to v3.x.
For information about removal of the system channel, see the [Create a channel without system channel documentation](https://hyperledger-fabric.readthedocs.io/en/release-2.5/create_channel/create_channel_participation.html).

**Support for 'Solo' consensus ordering service has been removed**

The 'Solo' consensus type was intended for test environments only in prior releases and has never been supported for production environments.
Support for 'Solo' consensus has been removed in Fabric v3.0.
For trial environments you can utilize a single node Raft ordering service as demonstrated in the [test network tutorial](https://hyperledger-fabric.readthedocs.io/en/latest/test_network.html).

**Support for 'Kafka' consensus ordering service has been removed**

The 'Raft' consensus type was introduced in v1.4.1 and has become the preferred production consensus type.
Support for 'Kafka' consensus has been removed in Fabric v3.0.
If you used Kafka consensus in prior releases, you must migrate to Raft consensus prior to upgrading to v3.x.
For details about the migration process, see the [Migrating from Kafka to Raft documentation](https://hyperledger-fabric.readthedocs.io/en/release-2.5/kafka_raft_migration.html).

**Legacy chaincode lifecycle has been removed**

The legacy chaincode lifecycle from v1.x is removed in v3.x.
Prior to upgrading peers to v3.x, you must update all channels to utilize the v2.x lifecycle
by setting the channel application capability to either V2_0 or V2_5,
and redeploying all chaincodes using the v2.x lifecycle. The new
chaincode lifecycle provides a more flexible and robust governance model
for chaincodes. For more details see the
[documentation for enabling the new lifecycle](https://hyperledger-fabric.readthedocs.io/en/release-2.5/enable_cc_lifecycle.html).


Deprecated features
-------------------

**Support for specifying orderer endpoints at the global level in channel configuration is deprecated and may be removed.**

Utilize the new 'OrdererEndpoints' stanza within the channel configuration of an organization instead.
Configuring orderer endpoints at the organization level accommodates
scenarios where orderers are run by different organizations. Using
this configuration ensures that only the TLS CA certificates of that organization
are used for orderer communications; in contrast to the global channel level endpoints which
would cause an aggregation of all orderer TLS CA certificates across
all orderer organizations to be used for orderer communications.

**Support for configtxgen flag `--outputAnchorPeersUpdate` is deprecated and may be removed.**

The `--outputAnchorPeersUpdate` mechanism for updating anchor peers has always had
limitations (for instance, it only works the first time anchor peers are updated).
Instead, anchor peer updates should be performed through channel configuration updates.

**The fabric-tools docker image is deprecated and may be removed**

The fabric-tools docker image will not be published in future Fabric releases.
Instead of using the fabric-tools docker image, users should utilize the
published Fabric binaries. The Fabric binaries can be used to make client calls
to Fabric runtime components, regardless of where the Fabric components are running.

**Block dissemination via gossip is deprecated and may be removed**

Block dissemination via gossip is deprecated and may be removed in a future release.
Fabric peers can be configured to receive blocks directly from an ordering service
node, and not gossip blocks, by using the following configuration:
```
peer.gossip.orgLeader: true
peer.gossip.useLeaderElection: false
peer.gossip.state.enabled: false
peer.deliveryclient.blockGossipEnabled: false
```

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric/releases/tag/v3.0.0-beta" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-03-14 15:24:50 +0000 UTC
    </span>
</div>

