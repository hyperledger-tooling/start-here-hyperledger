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
                    v2.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.4.1
                </span>
            </td>
            <td>
                v2.4.1 Release Notes - December 17, 2021
========================================


Improvements
------------

**peer - Chaincode as a service builder delivered with Fabric release artifacts and in fabric-peer docker image**

Starting in v2.0 chaincode can be run as a service by utilizing the external builder pattern for chaincodes.
Running 'chaincode as a service' has advantages in Kubernetes and other deployment environments since the chaincode can be managed independently rather than requiring the peer to build chaincode images and start chaincode containers at runtime.
The external builder pattern required you to deliver a builder script or program alongside the peer.
Starting in v2.4.1 an external builder for 'chaincode as a service' is available in the Fabric release artifacts and is pre-configured with the fabric-peer docker image,
removing the need to build your own external builder and repackage and configure the peer.

**peer - Gateway service now randomizes endorsement layouts**

For improved load balancing of endorsement requests and fairer workload distribution across organizations,
the gateway service now randomizes the peers it connects to for every transaction.

**peer - Gateway service concurrency limits**

Add support for setting gateway service concurrency limits, similar to how concurrency limits are
set for the existing endorser and deliver services.
Concurrency limits ensure that a peer does not process more than the configured number of requests,
reducing the chance of a peer getting overloaded with more requests than it can process.
The peer's core.yaml 'peer.limits.concurrency.gatewayService' setting defaults to 500.

Fixes
-----

**peer - Fix for orderer endpoint updates in channel configuration transactions**

When processing a channel configuration transaction, the gateway service was setting orderer endpoints based on the
prior configuration and therefore the gateway may attempt to submit transactions to outdated orderer endpoints.
A peer restart was required to refresh the orderer endpoints.
The gateway now sets the orderer endpoints based on the updated channel configuration without a peer restart required.

**peer - Extraneous warnings logged for service discovery endorsers requests**

The 'discovery.acl' logger was logging an unexpected "identity does not satisfy principal" warning message.
The message has now been removed.

**peer - Improve gateway service memory garbage collection**

Remove duplicate proposal responses from gateway service memory to improve garbage collection and peer process memory footprint.

**peer - Reduce the size of gateway service gRPC error responses for non-matching endorsements**

The gateway service was returning error responses with full payloads to clients when it received non-matching endorsements from peers.
Large error responses in gRPC can cause loss of connection between client and server.
A shorter error message is now returned to the client, while the full payloads are reported in the peer log as a warning.


Dependencies
------------
Fabric v2.4.1 has been tested with the following dependencies:
* Go 1.16.7
* CouchDB v3.1.1

Fabric docker images on dockerhub utilize Alpine 3.14.


Deprecations (existing)
-----------------------

**Ordering service system channel is deprecated**

v2.3 introduced the ability to manage an ordering service without a system channel.
Managing an ordering service without a system channel has privacy, scalability,
and operational benefits. The use of a system channel is deprecated and may be removed in a future release.
For information about removal of the system channel, see the [Create a channel without system channel documentation](https://hyperledger-fabric.readthedocs.io/en/release-2.3/create_channel/create_channel_participation.html).

**FAB-15754: The 'Solo' consensus type is deprecated.**

The 'Solo' consensus type has always been marked non-production and should be in
use only in test environments, however for compatibility it is still available,
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
If prior versions are utilized, a Warning will appear in peer log.
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
are used for orderer communications, in contrast to the global channel level endpoints which
would cause an aggregation of all orderer TLS CA certificates across
all orderer organizations to be used for orderer communications.

**FAB-17428: Support for configtxgen flag `--outputAnchorPeersUpdate` is deprecated.**

The `--outputAnchorPeersUpdate` mechanism for updating anchor peers has always had
limitations (for instance, it only works the first time anchor peers are updated).
Instead, anchor peer updates should be performed through the normal config update flow.

**FAB-15406: The fabric-tools docker image is deprecated**

The fabric-tools docker image will not be published in future Fabric releases.
Instead of using the fabric-tools docker image, users should utilize the
published Fabric binaries. The Fabric binaries can be used to make client calls
to Fabric runtime components, regardless of where the Fabric components are running.

**FAB-15317: Block dissemination via gossip is deprecated**

Block dissemination via gossip is deprecated and may be removed in a future release.
Fabric peers can be configured to receive blocks directly from an ordering service
node and not gossip blocks by using the following configuration:
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


## Changes:

* af5d5df427d41dd1a8e83bdeeff79086be2b2060 v2.4.1 release commit
* ef5ac00599d82f6067e5f253db65710d150ae665 Update 'Running a Fabric Application' tutorial for Fabric Gateway
* 3580b4e845769a5218a0f1f0fed181c78b5a9769 Reduce CPU&memory cost of collecting endorsements
* fbfdc1daac851ba36a5be938921b96992afee30f Enable gateway concurrency limits
* 1f877095649ec9968db93ae81ff83825ea07911d Remove discovery.acl principal warning [ #3006 ]
* e0bb139ccaddeaa329a6ed814fa30e7263413dd3 Adding a dedicated external builder
* 654a02b11bbd9290345da06ad33ea344d0bb379c Fix channel config callback in gateway
* abf5d3043e618bab17bfc2d5f79f59c425c4534f Final peer for gateway (#3091) (#3095)
* 2d8d7f405ca677f3da18850a0476c9c085e5b3ff Randomize endorsement layouts
* 29d1e2137b04a10f1e1c954cd2ba7fbdfd101c0b Network and Orderers for gateway
<details><summary><b>See More</b></summary>

* a95a8e72847bfa650757d80b8abbd7e32cd4bebe latest PR review comments

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=45483&view=logs).</details>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric/releases/tag/v2.4.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-12-17 12:42:25 +0000 UTC
    </span>
</div>

