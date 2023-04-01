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
                    v2.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.5.0
                </span>
            </td>
            <td>
                v2.5.0 Release Notes - March 31, 2023
=====================================

New features
------------

**Purge history of private data**

While it has always been possible to delete private data from current state, this new feature enables purging the history of private data from a peer while preserving a hash of the private data as immutable evidence on the blockchain.
* Useful for purging private data on demand for privacy reasons or to adhere to government regulations.
* Deletes private data from state and from peer’s private data history so that it can no longer be queried from block events or from other peers.
* Available as a new chaincode API `PurgePrivateData()`.
* Requires setting application capability to `V2_5` in channel configuration

For more details, see the [Private data documentation](https://hyperledger-fabric.readthedocs.io/en/release-2.5/private-data/private-data.html#purging-private-data).


Improvements
------------

**Multi-architecture binaries and docker images are now available**

The release binaries and docker images have been updated as follows:
* Support for amd64 and arm64.
* Release binaries are statically linked for maximum portability.
* Docker images utilize dynamically linked binaries and are now based on Ubuntu (rather than Alpine) to make them more consistent with typical production runtime environments (production runtime environments are typically based on glibc and often require dynamic linking of HSM modules).

**Orderer configuration SendBufferSize now defaults to 100**

Orderer configuration SendBufferSize default has changed from `10` to `100` to improve performance of large workloads.

**Peer gateway service now supports seamless resumption of chaincode event listening**

Client applications can now resume chaincode event listening after a disconnect and reconnect without receiving any duplicate or missing events.
The client must specify an AfterTransactionId property in addition to a start block number when requesting chaincode events in order to ensure no duplicate or missing events are returned.


Fixes
-----
All fixes as of v2.4.9 are also included in v2.5.0.


Dependencies
------------
Fabric v2.5.0 has been tested with the following dependencies:
* Go 1.20.2
* CouchDB v3.2.2

Fabric docker images on dockerhub utilize Ubuntu 20.04.


Deprecations (existing)
-----------------------

**Ordering service system channel is deprecated**

v2.3 introduced the ability to manage an ordering service without a system channel.
Managing an ordering service without a system channel has privacy, scalability,
and operational benefits. The use of a system channel is deprecated and may be removed in a future release.
For information about removal of the system channel, see the [Create a channel without system channel documentation](https://hyperledger-fabric.readthedocs.io/en/release-2.3/create_channel/create_channel_participation.html).

**FAB-15754: The 'Solo' consensus type is deprecated.**

The 'Solo' consensus type has always been marked non-production and should be in
use only in test environments; however, for compatibility it is still available,
but may be removed entirely in a future release.

**FAB-16408: The 'Kafka' consensus type is deprecated.**

The 'Raft' consensus type was introduced in v1.4.1 and has become the preferred
production consensus type.  There is a documented and tested migration path from
Kafka to Raft, and existing users should migrate to the newer Raft consensus type.
For compatibility with existing deployments, Kafka is still supported,
but may be removed entirely in a future release.
Additionally, the fabric-kafka and fabric-zookeeper docker images are no longer updated, maintained, or published.

**Fabric CouchDB image is deprecated**

v2.2.0 added support for CouchDB 3.1.0 as the recommended and tested version of CouchDB.
If prior versions are utilized, a Warning will appear in the peer log.
Note that CouchDB 3.1.0 requires that an admin username and password be set,
while this was optional in CouchDB v2.x. See the
[Fabric CouchDB documentation](https://hyperledger-fabric.readthedocs.io/en/v2.2.0/couchdb_as_state_database.html#couchdb-configuration)
for configuration details.
Also note that CouchDB 3.1.0 default max_document_size is reduced to 8MB. Set a higher value if needed in your environment.
Finally, the fabric-couchdb docker image will not be updated to v3.1.0 and will no longer be updated, maintained, or published.
Users can utilize the official CouchDB docker image maintained by the Apache CouchDB project instead.

**FAB-7559: Support for specifying orderer endpoints at the global level in channel configuration is deprecated.**

Utilize the new 'OrdererEndpoints' stanza within the channel configuration of an organization instead.
Configuring orderer endpoints at the organization level accommodates
scenarios where orderers are run by different organizations. Using
this configuration ensures that only the TLS CA certificates of that organization
are used for orderer communications; in contrast to the global channel level endpoints which
would cause an aggregation of all orderer TLS CA certificates across
all orderer organizations to be used for orderer communications.

**FAB-17428: Support for configtxgen flag `--outputAnchorPeersUpdate` is deprecated.**

The `--outputAnchorPeersUpdate` mechanism for updating anchor peers has always had
limitations (for instance, it only works the first time anchor peers are updated).
Instead, anchor peer updates should be performed through channel configuration updates.

**FAB-15406: The fabric-tools docker image is deprecated**

The fabric-tools docker image will not be published in future Fabric releases.
Instead of using the fabric-tools docker image, users should utilize the
published Fabric binaries. The Fabric binaries can be used to make client calls
to Fabric runtime components, regardless of where the Fabric components are running.

**FAB-15317: Block dissemination via gossip is deprecated**

Block dissemination via gossip is deprecated and may be removed in a future release.
Fabric peers can be configured to receive blocks directly from an ordering service
node, and not gossip blocks, by using the following configuration:
```
peer.gossip.orgLeader: true
peer.gossip.useLeaderElection: false
peer.gossip.state.enabled: false
peer.deliveryclient.blockGossipEnabled: false
```

**FAB-15061: Legacy chaincode lifecycle is deprecated**

The legacy chaincode lifecycle from v1.x is deprecated and will be removed
in a future release. To prepare for the eventual removal, utilize the v2.x
chaincode lifecycle instead, by enabling V2_0 application capability on all
channels, and redeploying all chaincodes using the v2.x lifecycle. The new
chaincode lifecycle provides a more flexible and robust governance model
for chaincodes. For more details see the
[documentation for enabling the new lifecycle](https://hyperledger-fabric.readthedocs.io/en/release-2.2/enable_cc_lifecycle.html).

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric/releases/tag/v2.5.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-04-01 16:43:17 +0000 UTC
    </span>
</div>

