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
                    v2.4.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.4.4
                </span>
            </td>
            <td>
                v2.4.4 Release Notes - June 17, 2022
====================================

Improvements
------------

**peer - Add a "gateway.responsechecker" logger for logging endorsement response differences**

To assist with troubleshooting when endorsement responses are different across multiple peers, the new "gateway.responsechecker" logger will log warnings indicating which parts of endorsement responses are different.

**peer - Enable gateway service to invoke system chaincodes**

The gateway service can now invoke system chaincodes such as QSCC when requested by a client application.

**peer - Enable resume of chaincode event listening**

Enables the client to (optionally) specify an AfterTransactionId property in addition to a start block number when requesting chaincode events, which causes chaincode events up to that transaction ID (inclusive) to be ignored and not returned to the client.
This supports resume of chaincode event listening on client reconnect without duplicating or missing any events.


Dependencies
------------
Fabric v2.4.4 has been tested with the following dependencies:
* Go 1.18.2
* CouchDB v3.2.2

Fabric docker images on dockerhub utilize Alpine 3.16.


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

* 1473ecae6451d82a068aa943f8df8cf1a7ce4864 Release commit for v2.4.4 (#3487)
* 6f4282b8149997129933bc2b967cd47fe758d270 Fix gossip unit test flake (#3215)
* a914ec3d6e4be1a8991439e3e782f79ba7f904b5 Bump Alpine to 3.16 (release-2.4) (#3472)
* 8ffd334ec5ec37228c26eae4881b317ef71d6a13 Locate correct block number for transaction ID in ChaincodeEvents (#3289)
* f64eea25dc877cd13d87a81fb3ee6932c85db3fa Refactor of ChaincodeEvents service implementation to support resume (#3283)
* 02d63c3bc1050758e6a50f0e8b7d57a3ff8e7466 Add -buildvcs=false for building binaries
* 60638b5432f2c49a19de1e0e0cd25ab9bbc8c856 Improved gateway error for transient data failure [ #3328 ]
* a6947faae11a9fffb9bc8b2ffe5666dbd01b200f Use any peer to evaluate system chaincode transactions (#3447)
* 135c268e984bec95940c0aa0629fc5c2c0e30a12 Improve response mismatch logging
* 29fea4f17c0c160656933690532d5faaa4335a8f Log proposal response differences (backport #3420)
<details><summary><b>See More</b></summary>

* 4c6ef91ddd217d17a709d2002298d35487be4e8d Bump CouchDB to 3.2.2 (#3369)
* c8f83e45eaecec340af5958f801ead51950f921d caas review comments
* 3c2c2f8d0ccaaa79bc4044d72bc1741ce0899e0e no mdash char supported
* 24e6f347c9de847fec232b80a480807cc4c9789f new caas page
* 6588ed27b679d1395e176a8844f64f5f74fa5ec9 Bump Go to 1.18.2 (#3423)
* e5ad0ef6db94c98a5b5181409a8a8b380f87b519 Update chaincode language parameter name
* ffbd37bf9c3a41a902f21e22f65bf63e85ad2aef Fix hyperlink
* 566a1a652e0ddde1eb60d68041c08add21450ab9 Fix warning log printing
* ae316aabbea95d6c323059a548f1b0cfc743e254 Properly handle concurrent building of chaincode packages
* 37cca191fa59e02cdb982b61114d3f6eabf1e59a Update cc_service.md (#3355) (#3366)
* 1c97ab14491756513250dc1d457f4f5683ba35f5 Node 16 and v1.4 libraries (#3357)
* f6e83361c5a5bf8a075f30809ec857dac05893b8 certs mgmt guide (#3307)
* f614fb5babe50fcc567211e3e35a7b00cf0225c6 Additional TLS troubleshooting information (#3346)
* 1fb499abdcb80a6670b966e2f990fedceb7e6965 Handle empty policies when traversing the policy tree in discovery policy analysis (#3335)
* 0396bf928709a434e4941ceccab497a5656fdb0e Ignore channel double creation during replication. [ #2931 ]
* 458345aaf4341695439f674dcd11d622f0995b19 Add in the CCAAS builders to the tgz package

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=53819&view=logs).</details>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric/releases/tag/v2.4.4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-06-17 14:19:47 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.2.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.2.6
                </span>
            </td>
            <td>
                v2.2.6 Release Notes - June 17, 2022
====================================

Fixes
-----

**peer and orderer - Handle TLS CA certificate expiry**

When any TLS CA certificate configured on a channel expired, peer and orderer nodes fail to start due to MSP initialization error "setting up the MSP manager failed: CA Certificate is not valid: certificate has expired or is not yet valid". MSP initialization now ignores TLS CA certificate expiration so that the peer or orderer can start up and receive channel configuration updates with renewed TLS CA certificates.


Dependencies
------------
Fabric v2.2.6 has been tested with the following dependencies:
* Go 1.18.2
* CouchDB v3.2.2

Fabric docker images on dockerhub utilize Alpine 3.16.

Deprecations (existing)
-----------------------

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
node by using the following configuration:
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

* e7dc57d84d66f3288391bb436a247dbf977f970c Release commit for v2.2.6 (#3488)
* 862ab4d82c1ef0206aa7593c52776e393b001372 Add logging for identity, policy, and signature troubleshooting (release-2.2) (#3483) [ #3006 ]
* b7aaeb8591d1d3ffc6865413628f7b9122176138 Fix gossip unit test flake (#3215)
* 2dc7d5cf78d9613081fe1a83c86c6d0fbaa94507 Bump Alpine to 3.16 (release-2.2) (#3473)
* 2d286f19e3f25caa64fe3a590ce8b58b5107363d Fixed Found Typos
* b24f2c0b0fc4b106990030f2df9ba64a3aa8f46b Add -buildvcs=false for building binaries
* dd3e96ef6b3d887ba209f4552ba770aa8dbb9979 Update 'Using Private Data in Fabric' tutorial (Backport #1875)
* 61561ddb6b769a13d90ae2bd30871a2238b6a94b bump Go to 1.18.2 (release-2.2)
* b17d01a723e8647f0ae29dd7c3424e2992c55736 bump golang.org/x/crypto and golang.org/x/tools (release-2.2) (#3436)
* 21e522bf0c6c493b0e0502ebbca89c3102cadf49 bump go-dockerclient (release-2.2) (#3435) [ #2338 ]
<details><summary><b>See More</b></summary>

* df783d63e2a9b45cd1820d9ed44b4b1e17922b27 Remove duplicated line
* eabe68b19517d5cddd3a3820a4c318e00495aa44 Fix some errors in the tutorial
* 4f618907fd509b94a1aeeaee1558856d3fb9c292 Bump CouchDB to 3.2.2 (release-2.2)
* 8be2067b4c2ae893c0e6b39a6f2c9b6c88942a6e Fix mistake change 'curl' to 'git'
* 2deacbaaf307ff66bbdb007983e6a66c8d4d0d55 Fix doc to handle $PWD containing whitepaces
* 6a1071e0c1fbb0f6e9acd846bf888ed6ca068307 Update README build badge link
* fa43e6111fbdd0d38deee684ddbe941a7fb8a224 Update links for Jira to GitHub issue transition in README
* 4b1bfbf96931a5b45aaaf5b11f7a46e31b693ff9 Update boostrap.sh for test network
* e7280018cfe8b30c11f6394601aaa3c1d7d81a22 Update documentation to include Go SDK
* 449ef0a41f4f422c5a32220e2703a2950af051af Fix link to security bug reporting process (#2160)
* 2f4eb7f293938c8104fcb99c0823032acd92b1c8 Update "master" branch references to "main".
* 09393f605d57f670b7d3dfa4b50a2ed5aeb67c9e Update chaincode language parameter name
* ed67dbe8c52de97cd03ca8a31f50a4d56563d558 Fix hyperlink
* 61d5840341fb5307aaf9595c8027928c2b2b32a8 Fix warning log printing
* 578a648bc8bca4b6d7ded3b24c2d50b308a85201 Properly handle concurrent building of chaincode packages
* cfbb980816b524095c9ed3728d1222011144638c Documentation: Update network (Key Concepts) page
* 0d79dd2fa512350440b804358f0b1b0b96b3fb64 certs mgmt guide (#3307)
* 0132f2aef32df964e1dde14f01509fc2207f43b9 Additional TLS troubleshooting information (#3346)
* 4ab905936be47bbe3e7ac16983baee2c54ab73a2 Ignore channel double creation during replication. [ #2931 ]
* e2f05e6cdb7b40e0226f893934b46def03b175cd Ignore expired CA/TLS CA certs on msp init (#3238) (#3249) (#3255)
* 68b6b90fe7aa6eb455c2f7b9a0b56ed1e74ff217 Fix FAB-18528: remove panic in ifConfig func (#2828)
* f7318ffd40215798f90e3944da74c706b717c746 Release commit for v2.2.5
* c04cd7d054a4e0d01855b804868c007cccb2455c Bump Go to 1.17.5 (release-2.2) (#3186)
* 4996e82df550e40d9381c60d423f50bca382d291 - Fix failure to generate all possible combinations (backport #3132) (#3150)
* 162f86717711dd3001fd737e8f5635993f9529e3 Add Information about AWS HSM
* fcdc0b59fa467d4105fe3a440d79174fb130c098 Backport setEvent information to 2.2 [ #2958 ]
* acf88a04e52dd80d49ac8d6eb219f59a96f61eb5 [Backport]  #2936  to release-2.2 (#2953)
* eddb470601248255bb52f0556a0900e2794d69e7 Unit test flake when rpc server stream not closed (backport #2935) (#2942)
* 19a137b2d8274057a99eace85f94140b28771306 Fix broken links for international workgroups (#2920)
* 2088b5fa2a340bc3e75df945c18b96df5b29f64c Update docs for Jira to GitHub issue transition
* 263ca9e1447c5c23c911fe9728994812eca8bd71 Release commit for v2.2.4 (#2901)
* 029e6ed2aea4db27953243efe7a7937000e1671a Fixed a typo in private_data_tutorial
* 1eedcff7b5f3583efc0f59078793f8559666e095 Update Go to v1.16.7 and alpine to 3.14 (release-2.2)
* 851f838e02849965a9b7aa33366821223fd4e4a7 Fix process termination waits in health tests (#2889)
* e6a6a61fdfaab844e8560d8192014b3b1970bda8 platform/golang: loosen assertion for Go 1.16.2 (release-2.2)
* ba2a9f1910d444bcb5e71d08173f583311b4202a deps: bump testify (release-2.2) (#2886) [ #2336 ]
* 50064c891c48143694a9a4abdce57f6f04796503 Update x509.CertPool equality checks (#2880)
* f441ba23542c4c21af18ff0829cae76ad56b1039 Change name of test network docker network in 2.2
* 859c7d53283febd9103cd90f93a2d7922ea3a8fa Clean up Go modules (release-2.2) (#2876)
* 07ac9f56a8ea352409c3d6200024fb1517118f20 Stop spamming for wait channel acquirement in orderer integration test
* b076bd7f09053353040f8149bb325804a22800d1 Options for GRPC message size configurable
* c91b5467ac12e173bce8cbe3498b119ceed948bf Change name of comm msg size default consts
* da9e1bd7a2214f2815bcc05e4cc6917447992498 Refactor max message sizes in comm client config
* fbf7b936f4347b9e0d398adb8e41a47d2b4a1497 FAB18529 added nil check in channel header parsing
* 9a6b35104e88dc2df08db7c7b0ba3d0f61127a85 Additional documentation for implicit private data collections
* 8fd2ad8c6e7d8cd92744c7efa31a451e1725bada [FAB-18509] Stop panic of collection index path is wrong (#2726) (#2744)
* 62c68d1d4de224100cde95a647202a69ea30ade1 Updated enrollUser function in write_first_app Doc (#2713)
* a0dcb5c32d963901c50bb2002b83722509ead07d Update docs to clarify that an implicit collection can not have an index
* 2f7fd17aa77d3c9f584c61ac65b3ba079c9b23ea Fixed grammatical errors
* f36fe03341761bc629278e957597ee9c36801c15 [Doc-Update] + What is a commercial paper section
* 8b1d35584af08a78b9646eec7c94831933bf6602 Fix a typo in CouchDB tutorial
* 4c77749b01a46e60d8a29f822a5e83c07fcfdd5e Fix typo
* f3f170fec8c7c18b058db5eebe77ba5d9b14fe69 Fix peerchaincode.md as well
* 30a093153049ed122a6c003d002bd96f98a525bf Add explanation of `--ctor` JSON string
* b926247b90f4eb8a0c7fc1d2f5da87ed65c375b6 Clarify orderers seeing the transaction data
* f4feedb87d821e9e7a2bc1a8e87a7e4f4599a3ef Cherry pick deploy CC fixes into release-2.2
* 68bc522ec7985a6d04a4ef7455d206ab860ee17b Clarify "identity expired" error messages (#2685) (#2688)
* 3a69034157103971844f755cd1db44aac7373afd Fix spelling mistakes in the Github Contributions page
* ccecf10de97c8c029fff063929bd93d2f2ff2977 [FAB-18484] Return transaction forwarding result back to the client synchronously
* 7e6194485bf4fc9b3f03872a6c84dbb4ab87163a [FAB-18487] Update broken link in 2.2 branch
* 186d9bf1781041d1c2c98a2a2dd13b1ebb04168b Typo fix in peer deployment guide in main (#2660)
* 31e41cebf3231f2ee26bb5b43168f638de88e61d Update private_data_tutorial.rst
* 4cb453e433014a50d8ff5f1b21a1fd57785136e4 Fix jq commands in create channel tutorial (#2662)
* 8851da3d2b5395dd3882597b2a10c1c99390c59b Back port 2023 - skip empty ledge and 2635 - RetrieveBlockByNumber (#2648) [ #2023, #2635 ]
* cc504514ea3958414cc16ab1015b8c9a32cca34f Clarify doc for readset validations (#2647) (#2655)
* 3548215d2e7cebe83d2417ea0eb71e7528802991 Update secured_private_asset_transfer_tutorial.md
* 56b3689059bf282a56ac1a20d6cdfd96c3b4edbf [FAB-18479] Log error if orderer can't forward SubmitRequest to Raft leader
* dd7e9210fcaeceee0f071d64f051425a5a11dd81 fix duplicate entry in code snippet
* 7871c2683fe6f5741b5debce409b9156bcc47963 Optionally disable gossip block forwarding (#2606)
* bce75cf5d9ba320515b22e70fbf70fb38ec6d5f3 Update docs/source/upgrade_to_newest_version.md
* 678523ba621eb707ba59f17fbd521e09ea804c80 Govendor added to documentation
* 26b45ca1c8c32db8a86502c5e31b5e9cb0a37c62 Deploy a chaincode to new channel command issue
* 3f2158a01ee40b8ce58572db46de0a0cef7b20a7 Improve error message for invalid consenter cert (#2587)
* 94ace6540955c488efd70eff6f33861ffc51d3d5 v2.2.3 release commit
* d27212277042d5040f642ddb5783a6e241fc688f Cherry pick removing duplicate word (#2523)
* 222fbc832872d26f0f4d069da17fe29ea0af554b Add Security Model topic to docs
* 81168727fca97686c706d475286f06cba3e38682 Fix link in `international_languages.md`
* 496c5f54763ddfcd6c06e473b7425afc70aa1bc1 integration: PKCS#11 SKI to CKA_ID mapping test
* d2d031e4fd73f3a0d057b3d18ab4aefeb8601d13 pkcs11: Add SKI to CKA_ID mapping for BCCSP [ #11 ]
* 7214be78f76691c604e47a4cb67933631a9695a1 Prevent race that occurs after test timeout
* 6adcbce42c98aa64661258034f6a4bb115983b7c integration: backport chaincode_server_test
* 88432235436d40d20aeb13e3c668cc31fc5f7ebb Back-fill tests for externalbuilder.Duration
* 796f760ddfbbe8c4445aa7ad0cf924f479dda616 This commit upgrades goleveldb. This upgraded version includes a fix for [ #2463 ]
* fae13c393be8c2e2f7463b20d0b7f46e3acee24f Report correct reason of stream abort in orderer cluster
* 2b2e15466e74485f105635e1594ba1eb98cd30c9 Log stream total lifetime
* 100a7e789ebea04972e453f2f1d9c5bc416ee586 corrected organization labels
* 6320aed4680774a43874577071922ebafdea145b corrected Org1 text in Org2 box to Org2
* 8d0645b63445951892261bb9f25b2d310a6376af Update build to use Go 1.15
* 6cb530b12f138df7f81d640af495336cebccb67b Change string cast of int value to rune cast
* d5392448774c77a6cf05e9c4a3be481a22cd2a40 Directives are in comment text instead of groups
* a1b4d2d17dd77325dc47ca5c51557060f9672654 Implement legacy name constraints verification
* 4321503deba382e317f182259b403e539ac91952 Add test to assert on name constraint behavior
* 880914cae46634136b6408ae2cf200cd8d84b013 Re-encode ECDSA CRL signature during MSP setup
* 8883d7161ac7a006caf5780566e520b7ce884c0c Add test to exercise signature validation change
* cb3c87b94e5cc3ec599854cac35b0bb819b76661 deps: bump github.com/pkg/errors
* f635afd92413c1b0ac9f76fb3eb84927f1ed7cb8 Adjust etcdraft error assertions for go 1.15
* 5f19a003462c27f308c4a0b0b77cfe49e8517183 Replace test cert fixtures with generated certs
* aa7ad4fea3f727ed5270380412e5b9b743a1cca0 Set SKI, support multi hosts, add Signer to CA
* 684e255ecd400fd4d4a42325f19daac3f5874aa5 Fix typos in a "Developing Applications" doc
* 358cba73009e44a477d72ca4b513072fbe9c4fa7 Update AZP Service Connection Name
* 913d2ab416ae18a139a0bbe3363ffce93c60522e Prepare for next release v2.2.3 (#2347)
* eb2b1ea39e93081a346db75fe081f6b830cd19b4 Add peer log message for failure to invoke chaincode (#2339)
* 0583c22501c8027c2a847cdfa2f352a1baca57ac Add test newtork download instructions to create a channel tutorial
* bebb75fd192ebbf54239eaed2470ade6aa766fee v2.2.2 release commit
* a80c7727d48e5f4c2e0d19e9bfc6e6158d4a2b3c Add release notes for v2.2.2 (#2232)
* 1de0825e72bb36753ae7c208afc3678190363915 Fix the issue of Nil/Zero-length-byte-array value (#2310)
* e5ecdef1cda476be144942d8435a576c08dd78bb Remove system channel from Test Network tutorial
* c25eb863ea334d21f0086be3eb07e6c676565ca1 [FAB-15648] document update: Non-TLS orderer with etcdraft usage (#1678)
* a861c002e883e158d9db3bd859afed6f682bb2c9 cherry pick test network doc chaincode deployment fix
* 10c7839798afb2c1303e7e487768fd2b600996d3 Remove unreachable and unnecessary code in gossip membership (#2295)
* 68055151b43cd3fd7ee46ee82a529b8fb7c25ce7 Orderer deployment tutorial update
* fba5d9038c089ce8b53afc61d1c01bda775f2635 [doc] fix broken link
* 48bad48fce57976c7867b170be2504df9bf8b4c2 [FAB-18170] Endorsement policy page discusses NodeSDK
* ee8fcfc126935f649f78a1e8c0c6abd96b88889c [FAB-18392] Clarify scope and limitations of test network
* 90326b8441a9ce1f72a72393fb5c688de1e2722a [FAB-18252] Documentation should reference Java chaincode support
* 813be7f95ded8d6eb330c1d8ade764aad7a981fb Remove anchor peers from configtx.yaml tutorial (#2257)
* 11526cffded9ad100d8d0e80e756b0e32ec08ae1 Cherry pick org3 edits to release-2.2 branch (#2256)
* 5953056d396077cfd5a7b25c2f203d5d32eb5807 Split command in "add an org to network" tutorial
* 91d9621761d422e8be8303184d8246bc4dc94ab1 Add more details to logging specification examples
* 7b1dbf116c567228ebcfe063c8e9703fc9e4b7cb Update image filter used by integration tests
* 2a8d96c9566d22da9875aa8ffa7ba69f8dd23977 Remove Short Names and Replace With Full Path in Fabric
* b2a5aece462d35600a1071bfcfe41bd035e8bcce Check correct error
* 73b39dc70ff748a5943cf2b8880a442ec623cf7d [FAB-18378] Log warning when peer is lagging behind and cannot catch up
* d5d99651c00bd40eadec4a525f1dc42b075a9540 [FAB-17039] Skip retrieving pvtdata from transient store when txid is missing (#2183) (#2201)
* 3496dfc7da109e29e1ea9efc3881911f68a53e3c [FAB-17954] Document CouchDB JSON determinism (#2187)
* 26cbec6051b48b1a3bbd9d89875cc98744bba06f [FAB-18323] CherryPick: remove ephemeral from BCCSP SW options (#1553)
* db9a56fc1647db940a141705c3a4c07f278e6c42 Fixes Hardened to Hardware
* a381654fbb9998bd5b867c84ea7f5000b738c11a remove repeated the
* bbaa5b8fade220c809238e6feba5cd70f50fd281 update private-data sample instruction for Asset owner string
* 82b4566e194a30ff59eca8abd811c1e4439e6112 Remove reference to first-network
* 0a1fc23c40cc91dc59fdd0c5e509a3c230c5cc60 [FAB-17727] Log warning if system channel has no consortium members (#2149)
* 935a5c2bc99b672c280c44d3e861d8b5d8e7849b Deploy production ordering service doc
* c92835951c5dec358553456bc636bb500a1db580 Add release note for RSA CA changes
* 50ca5d45b42861e2ec3781ed8d5ce059075ef8ed Add integration test for MSPs with RSA CA certs
* b3646e5974506c797a32580f515f6d8f05220310 Restore RSA support for x509 public key import
* 40264135a126ad7ba708e576444d0e7788380482 Add check for invalid key before hitting couchdb (#2133) (#2135)
* b8a095f9cf8ef75d664f7e6af4d414f0723c760b Add persistent volume note to peer deploy guide
* bf2ebb609d7a245178d30fc21d24e8fb8c8a4b80 [FAB-18298] Default cluster cert and key (#2119)
* cae9a63b5dd54adef10e4a27a93e24a87e675f6f Update Go to 1.14.12
* b247ed42807b9c3b3a96b299c52a76f93dc6609b Revert "Allow BCCSP config to be set using env var (#1900)"
* d1b45245e0a98adcc06f040cf596dfdcb653ff97 Update Jira instructions in contributing guide
* d1730da2862f036787d4394aa8e9df19e352912c Cherry pick [FAB-18290] Add channel name to pvtdata reconciler log msgs (#2091)
* 99c2d1212761fbea420435aad863d13ea6695e00 Deduplicate orderer server TLS root CAs
* 1e15b6441f5abf01070c9895bb31b64f737a7f57 Log TLS handshake duration
* 9c5b283abaca47d405bc61f701632a6514cc430a FAB-18244 single node catches up with snapshot (#1964) (#2021)
* 09234c0b7ae23c99abe3cb4ce7eb495cfa69b077 Remove common name from private data doc
* 5a373061b4c7a38048392d55c1016043485363fc Fixed TLS certs validation for consenters (release-2.2) (#2005) [ #1888 ]
* 6f3ad12b3d4c6b76c1d12f8edb0a15c042101745 [FAB-18270] Disable debug of CouchDB response body
* 4d40d651c0e64e5e8b1bccb645ddb3b8b7815baa Peer deployment guide
* 70c41c1b19e3d403a4eedd4db9eb9e0fe9aef2cd Update help text in test net tutorial
* 8930c8c2d2e9b3093e945007543e150839073f17 Fix Node OU error message
* ab7104a8972d65437138d40b7361806bfc5e8ebf Update release docs
* 4a636426c5034aecd395b6f3d3e0030d5104b3d6 Cherry pick private data tutorial rebase
* e36ca2995528b779af3342a1af1a0e94b1803c05 Add Troubleshooting topic to Test Network for Docker Desktop setting
* e05c443389010ef56d3a5bf3f1cb46ed3dd11749 Allow tick interval override via orderer.yaml
* 32cb396f4786aa7b509cd75dfa4427d4209cd0f3 Fix chaincode lifecycle tutorial invoke
* ceb23df8c5477adec49d7eb47f4118b096d54adf Always Finalize the PKCS11 FindObject Operation
* 2d59f180bbeab330822e3c011491cacea1c5474a Corrected to capitalized function names.
* 6a370f73ee46073c5671b61778981517bfbceaf9 Fix table width issue
* f2e9e6e7b307a25dc4738e97a1ffb08daea4f6dc Allow BCCSP config to be set using env var (#1900)
* 6bd0699c7e7e6712bbd6b1ac4be32d34cdf81176 Exercise a full end-to-end flow with PKCS11 (#1717)
* 0b3b95fd58eb6bcb969a30218b12297ac68d5fab removed unused variable
* bf0b300aea9aebf6127996d54755c67ba7b99b89 [FAB-17129] Configure peer and orderer to use PKCS#11 as BCCSP in integration test
* 8407bc8af75326951465d117b2dbb66de5632cec Prepare for next release v2.2.2
* 74ac27cc15e60b4ed9ba94422478e3bb4bee81c3 Add two and three digit publishing
* 344fda602252cf1de6b1231341b65465edde56ee Release commit for v2.2.1
* bebb5d812ee84c1250bb4632cccf602893c6d45d Cherry pick secured asset transfer tutorial to 2.2
* ba9eaff56adbceb609db153577f46e3d10f6c74b [FAB-18041] Add Node.js to CC as external service
* 107a8670079efd548a157341f06383cc706c0b78 Remove No Longer Relevant Release Note
* 99a01b26070a455975c65b028ec0b6e89c635e7f Update release notes with FAB-18250
* 7b7ad6b3e4d6ac71087ae52e071be24048017427 Fix missing word
* f9f3caffe29b0d276a0f3a54123e9e0a3b2ab6ac Add change in documentation to explain how to add collaborators in translation
* 61c05b81f64c9de53ebec33d630a9e48d87475de [FAB-18250] Check Error Before Returning Session to Pool (#1937)
* 765bb73e3ac11e1dccf6d2a388cc1a07f1ad28be Remove escc and vscc from list of system chaincodes
* 99066433d561b5069f1884caf1a563abccc40238 Update v2.2.1 release notes with latest fixes
* c5cf62725d506015179b147275a4410c3d5fb872 Fix empty address in peer CLI ClientWait log
* 75046cf57c79da50033d9bc0d4c6e88bd4c64d6b Remove GetSessionInfo Call
* 2e4527b46d255cd1703e1e328d675bfcaf730541 Bug Fix: Saving big payloads by cache CouchDB (#1909)
* fe684f8a9908ac260ec7fcdd5ea6a840e6b9fc82 Fix flakey raft/cft integration test
* e2fa653e022c01188afe24df2e3300ba2ba037bd Add release notes for v2.2.1
* 6b1ac6fd73e30958f37390e1c69e5b5a57a7f5ac [FAB-18237] always update stateInfo message upon chaincode update
* f32cb81f1bd410edac0c29970a51b90983bdcef4 Bugfix in collection config history mgr (#1904)
* 3ee47a71683848faa7433d41bbd8aaacdc133b12 fix function name typo in store private data command
* ffcbf2550a965f54815319e30d633c398c228780 Clarify tlsHandshakeTimeShift CLI help text (#1894)
* 673c3646aa57b06c502dbde33459cd8c7d3300e6 Correct the explanation for signcerts in Membership section
* 68d13edbf435bb08e28be38340541df1b941e2c6 Update write_first_app.rst
* dc8660b31deee9b742c2a6aa7f76216690f29e89 Regenerate peer CLI docs
* 6c9abf9109096eb9d00102d4c328cd54c85d9a3e Peer CLI communicate with orderers with expired TLS certs (#1863)
* 6f764089352ca49896379565c1fd624aa17602df Bump fabric-config dep to 0.0.7
* c5c11056a764942ee26d1984738b369df431af08 address review comments (#1890) (#1893)
* a5a6acdeeecf0f445c67e19fd5ef0cd64803750e pass unreconciled missing pvtdata to pvtdata store (backport to release-2.2) (#1886)
* ee2bc1b54691b7aba45ef32a1b1acb8ce2c4caf4 pass unreconciled missing data info to ledger from reconciler (#1797)
* bc00758a82d9ded54daeb09127ad8182230502b5 construct unreconciled missing pvtdata (#1699)
* e500de98633a35c459dbb9dbaae3a6ebc686197b deprioritize unreconcilable missingPvtData (#1721)
* 10cb4eafd11c224885ebeddb550756aed03e5e3f mv oldpvtdata commit to separate file
* 7eaead1c5fcbe9fc5e1fd75883f6a7c571efa811 refactor pvtdatastore
* 659fe39b3fba9746bf70bfefb83b842c5e4e2f35 Adding notes for the usage of script during samples install
* 2d895c4f1232ef96cc5c97d567766f510430ec26 [FAB-18208] Do not sign gossip message if membership is empty
* 42da96350539a740cd624899cfc807e1eb569fc4 Convert Azure Pipeline To Stages (#1874)
* 6a0255971a95c5e784db45dd85a1293720807cf9 Fix data race in gossip/discovery test
* 7dcd9fd770da17ace2a9c3586d76d20777dfa0a6 Minor doc fix to clear Sphinx local build error
* 09764d8cc1c7930bcd3d53cd4e4934f73e5d2dca fix missing err check in the block commit path (#1543)
* cc6dc99273f5da3cad2c9c6dcb1c0e7fed2b47d1 minor cleanup of pvtdatastore
* 20f06973930dea9eecbd94ef48863af8c297580d reset leveldb batch after the commit
* bebe131d58325f8afd89dfeeb161db59ef80be73 Use directly leveldb batch (#1507)
* 99332daacc649a26446e701f034f6c406bd34ab9 [FAB-18194] Fix service discovery for legacy installed chaincodes
* 0bd0ab27df465caa8c2d9dddcbd7da15cb677172 Update RTD Placeholder
* ef2632eee53b3de33e247d9100a468250da021ac [FAB-18191] Remove contents of leveldb dir instead of the dir itself when dropping dbs (#1828)
* 8dae484118c4867fb9e9e37bb081dc7ec507aee5 [FAB-18120] Adding DevMode integration test for new lifecycle.
* 9da753a04e3dbf7d5849dc44bff241d2c6a503b5 [FAB-18169] Add DevMode support in ChaincodeEndorsementInfoSource
* 8bbedb8ae249d3db9ddcfb4a2b7f387461239a83 Revert "[FAB-18183] Bump sphinx in requirements.txt to v1.8.5"
* bf8f6fc7164f8767bf55bd0fa02b3fb6116130d1 [FAB-18188] Log orderer and peer cert expiration date upon startup (#1804)
* 0e52fffae60b324b52939d667c58664dce61f4ac [FAB-18171] Disregard certificate validity period in intra-orderer communication
* 445b997f66bcbda77a5e2ebe18919cb1d09c7a26 [FAB-18183] Bump sphinx in requirements.txt to v1.8.5
* 2fc575cbe2b7ec546659323cc8304f2e1c77599a Cache bccsp keys generated from getECKey
* 7b8de81ada3ee68bc92c78e3a2241ede8901fca2 Add object handle cache to PKCS#11 bccsp provider
* bf2f3fc530815b961abb5ef99bfb42d2ec349148 Make ecPoint a method on impl
* 2a2216067faca1219683acf19aefbaaf798efa02 Make findKeyPairFromSKI a method on impl
* 86a5c64219761a96365e6989da2f1dfc6f0d313f Replace loadLib with initialize method
* 8a637325607c7f3d2a611be9b27653a8eb23d306 Merge pkcs11/impl.go and pkcs11/pkcs11.go
* f47ac7d8e49d78d9a33a7d5525d2f434b177f96d Drain session pool before creating new sessions
* 4fd232ec13c26065de5cd9812335e0bcbba6280c Add instructions for how to use @Mergifyio backport command
* 2d522b5d2e9e9fde0ce7fcd711cf2cd70ca25fe0 Update Add an Org to a Channel tutorial
* 2813aba20dcae820af5c95ff68a64be90b2605ba Updates to CouchDB doc tutorial
* 4919fa7e04142034a4243b6d45546a8925186fc5 Updated Using CouchDB to use asset transfer ledger queries smart contract
* 64c7600cb6eec54710ce58d7798c65b752fccbbb Update Channel Update (Adding an Org) tutorial
* 7d6bb0f59a7b92e70fafb2efda450796d320090f Update docs to replace fabcar references with basic asset transfer
* 1450e3c2aa1a05e554396b2c11ca5b47ea40f48c Add links for Go and Java sample applications
* b8b7af74128d2d5e0db4c00be6da6b1ce258cd97 Refactor tutorial to 'Writing Your First Chaincode'
* 14ad1d7a1699e1ce27daf01599c289c91220c1c2 [FAB-18109] Update peer chaincode invoke
* e0426571d1ab56618239bf895c84f63e0058d05c Fix code snippet display (#1759)
* 9783edbb3b4dfa3059231c16d043fc110ed6b3a9 Write Your First App tutorial updates (#1757)
* 95635186d3f131699dd7127e4929d312c38280a4 Update "Deploying a smart contract" tutorial. (#1756)
* 417bcd40a84603ffb79837a78fdc8c25659cdb57 Update "Using the Fabric Test network" tutorial (#1755)
* 0b598c4e433764825d60862e4e693d2ebdcba14a Update Write Your First Application Tutorial (#1754)
* c4e310d7f31ba771b22807014dd76cbf347b5708 Remove Use of Manifest Tool
* 5f16da833f2fcb1d3061896e378fe2815bf9e51e Update RTD to Target Correct GH Release Branch
* 6491f6a3c92f69690c6320bf74c83a7632744172 Fix and improve discovery TLS authentication comments in document
* 50aea5e3468b6675ff3c09c4298c1680774ecfe1 Update doc to reflect change in FAB-18163 (#1729)
* 25a5c4011aa7a20708af9b299681a4c528741712 FAB-18163 TLS Timeshift w/o Separate Cluster Port (#1724) (#1725)

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=53824&view=logs).</details>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric/releases/tag/v2.2.6" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-06-17 14:31:24 +0000 UTC
    </span>
</div>

