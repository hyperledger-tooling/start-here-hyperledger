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
                    v2.2.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.2.4
                </span>
            </td>
            <td>
                v2.2.4 Release Notes - September 8, 2021
========================================

Improvements
------------

**peer - New configuration option to disable gossip block forwarding**

If all peers in an organization explicitly set `peer.deliveryclient.blockGossipEnabled` to false,
no peer in the organization gossips blocks to any other peer in that organization.
Use this setting when all peers pull blocks from ordering service. For more
information see deprecation announcement below: **FAB-15317: Block dissemination via gossip is deprecated**.

**orderer - [FAB-18484] Return transaction forwarding result back to the client synchronously**

With this improvement a Raft follower waits for the transaction to be forwarded to the Raft leader,
and returns the result (success or failure) back to the client accordingly.
Prior to this improvement, the Raft follower returned success after enqueueing it into the message queue,
which might have resulted in the transaction being dropped but a success being returned to the client.
Application clients should still monitor transaction commit events, since the Raft leader is not guaranteed
to deliver the transaction into a block in exception scenarios, but this improvement avoids
transactions from being dropped when there are connection issues between a Raft follower and Raft leader.

**peer and orderer - Make gRPC maximum message size configurable**

This improvement makes gRPC maximum message size configurable in peer and orderer.
Previously the maximum message size was hardcoded to 100 megabytes.
Since all nodes should be consistent it is recommended to keep
the default value of 100 megabytes for MaxRecvMsgSize & MaxSendMsgSize.
The value can be configured if needed however.
Configure in peer core.yaml with `peer.maxRecvMsgSize` and `peer.maxSendMsgSize`.
Configure in orderer orderer.yaml with `General.MaxRecvMsgSize` and `General.MaxSendMsgSize`.


Dependencies
------------
Fabric v2.2.4 has been tested with the following dependencies:
* Go 1.16.7
* CouchDB v3.1.1


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
<details><summary><b>See More</b></summary>

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
* f60c78a2b9bb3901c2029441174b04c8b0102dbd Add Raft metrics to Raft config doc
* c932bb434d122360478a032eef499a58022aec53 Use correct gossip SecretEnvelope reference
* 2821cfcd18e0ffb06508286fed0ca0a417993e2f Log Error When PKCS11 Key Not Found (#1679)
* cce8553816df3a9f83797d01d3c51930b8030942 fix: modify certificate alternate DNS duplication
* 6e97dd08a7d57fb7cabb23a5adc3aebb568e67f6 fix glossary.rst by reverting commit 21fa6480b161
* 8d590c6aa48df7fb4da406845910e911a5ed4082 typo fix
* 05655d0b9c0be21696432b4bf08dcf1dc2b65fc8 Fix link in Develop apps doc
* 67ce3cb752a98734cd728fd570ce4d572f7cf9b5 Fix: Missing addToWallet.js in ls command output
* 534e87a79b0eec21a180f5c7030faed99926011a Add link to Use a CA to deployment guide
* 9099e5b9baa0b1b37058bdfe166067d9e8133fd2 Fix international language make html instructions
* 3741860ac90f48ffb2ec77fa2fc22bad6e7cd6bf Raft: Check suspect info once per suspect interval (#1600)
* 03f0544a5f15ff0a1d476471ec1bd775ebbcf45e Add LTS release status to What's New doc.
* 6be80ae4c1c03c343a887609d24ac96e0ab1f91d Print channel name in learnAnchorPeers
* dd556f36b36f0a7a83ab7b18bdd1589b870b473a Advice for translators, PRs and tools
* 5dc22d54c549af2b5cc0500fa90aeea470f95507 Remove ccenv dependency in platforms unit test
* 9bca8d60c67d2755e7542021be4a3fc22d05f172 Changes for i18n
* 5f11b9b2ea41ee53acf0cd574b8b1eba4abbf608 Simple Typo fix
* 5ea85bc541c410b80ab9585d64f5ba13567c162b Fabric v2.2.0 release commit
* 7b1a1a20f64c52ca5a5a2e8e9d9bfe0bd2d82bd1 Add release notes for v2.2
* d2dfc63b00e1cb82da593bbcdf164be1aef86c29 Improve peer CLI error message when no orderer address passed (#1555)
* 9c3c599f832f4b727d3d1cb1fffa4a16c8669161 [FAB-18054] Remove default value for top level orderer addresses if (#1550)
* ff00d9b225b62c1f5605893b512115fecbdc2e6d Improve private data logging (#1545)
* 62dfb2deefd0995a5b067026b1302572da1b567e Add org name to consortium error message
* 0de7fc1486a53923c1f97ac266b3f49a7d05e00f Restore couchdb logger (#1532)
* 2169710b4469d13d3c0eb6ac341e8222aa462661 Use tcp for statsd and poll for metric arrival
* 568d346ee6046fed3386fc8e140291724bded345 Fix chaincode package example path
* ac3f596aff12b2ebb94d128add8ad86f0bd0253f Remove Thirdparty Images From Bootstrap Script
* 9b187f5bb9cfc2273963172f43cbe41f26611e2c Edits to style guide
* a6ad40786a4b68c59ea4e97af44d7b94afdabdec Upgrade updates
* 8fd785a5b5f4e104457b45c4cb2b81839e1a7672 Deploy Chaincode Doc
* 4591d52fdd7cc4b7f5378e37fc3f681da046426c Add Check For CouchDB 3.1 (#1491)
* 529a9314a640c569ae170a60c630ede2f186b37b Only canonize ECDSA signatures in MSP:IsWellFormed (#1498)
* 3d305f7f1614c3272f9af1fccb1667814b3d75f7 Disable channel participation API in release-2.2
* a7dc1d41fd4efb101e5ec9233a590bc359526087 [FAB-18028] Create new PropagateEnvironment key

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=40699&view=logs).</details>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric/releases/tag/v2.2.4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-09-09 06:43:03 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.3.3
                </span>
            </td>
            <td>
                v2.3.3 Release Notes - September 8, 2021
========================================

Improvements
------------

**peer - New configuration option to disable gossip block forwarding**

If all peers in an organization explicitly set `peer.deliveryclient.blockGossipEnabled` to false,
no peer in the organization gossips blocks to any other peer in that organization.
Use this setting when all peers pull blocks from ordering service. For more
information see deprecation announcement below: **FAB-15317: Block dissemination via gossip is deprecated**.

**orderer - [FAB-18484] Return transaction forwarding result back to the client synchronously**

With this improvement a Raft follower waits for the transaction to be forwarded to the Raft leader,
and returns the result (success or failure) back to the client accordingly.
Prior to this improvement, the Raft follower returned success after enqueueing it into the message queue,
which might have resulted in the transaction being dropped but a success being returned to the client.
Application clients should still monitor transaction commit events, since the Raft leader is not guaranteed
to deliver the transaction into a block in exception scenarios, but this improvement avoids
transactions from being dropped when there are connection issues between a Raft follower and Raft leader.

**peer and orderer - Make gRPC maximum message size configurable**

This improvement makes gRPC maximum message size configurable in peer and orderer.
Previously the maximum message size was hardcoded to 100 megabytes.
Since all nodes should be consistent it is recommended to keep
the default value of 100 megabytes for MaxRecvMsgSize & MaxSendMsgSize.
The value can be configured if needed however.
Configure in peer core.yaml with `peer.maxRecvMsgSize` and `peer.maxSendMsgSize`.
Configure in orderer orderer.yaml with `General.MaxRecvMsgSize` and `General.MaxSendMsgSize`.


Fixes
-----

**orderer - [FAB-18521] Consenters' metadata is not replicated while OSN catches up with snapshot**

If an ordering service node crashes while replicating blocks from another ordering service,
the consenters metadata will not be available and the ordering service node will not be
able to reconnect to the consenter set upon restart. This fix ensures that an ordering
service node that is replicating blocks persists the consenters metadata so that it
can reconnect to the consenter set.


Dependencies
------------
Fabric v2.3.3 has been tested with the following dependencies:
* Go 1.16.7
* CouchDB v3.1.1


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

* 99553020d27768103e6cae2947ed6e96a7a7d08d Release commit for v2.3.3 (#2903)
* b5eb7f0efd4c86e6386ce6ef1cf61c1975c596e0 Fixed a typo in private_data_tutorial
* 5be686fcb3d1a00662ff6593778af5937a32fb14 Update Go to v1.16.7 and alpine to 3.14 (release-2.3) (#2874)
* 0ebd9cfb16534a24e03cff6609b7d121a75041ff platform/golang: loosen assertion for Go 1.16.2 (#2480)
* c5c1accb73bc74b238fbebd5d117fd1b7bdf521e deps: bump testify (release-2.3) (#2885) [ #2336 ]
* cf3470b69ed0ea12363ceb20f17a0b79558fcbf6 Update x509.CertPool equality checks (#2879)
* 67d3523b1323506850a85088c46614c1c045bca0 Clean up Go modules (#2875)
* 758735be161fca864180463d229cc919455f1971 Stop spamming for wait channel acquirement in orderer integration test
* 497d3abea7e472daccb753ae9aa7ab173ef5ef9c Options for GRPC message size configurable
* cc88dfa7c990deef9304aed1173d7009b9cd6d01 Change name of comm msg size default consts
<details><summary><b>See More</b></summary>

* 8956c06395e5d009fa3b99c5ea7c97b5fd9e9245 Refactor max message sizes in comm client config
* befdaeecd8b821774ff9bd4da1ac09dc59d0a220 FAB18529 added nil check in channel header parsing
* c1b298d9f05b88868966f216aca213bcdf1f55b7 Fix small doc errors (#2816)
* 9815a7a8f0f72e1ae41a3e35e5272e3dd4a38c28 Update private data docs - remove SDK reference (#2770)
* 1294920d4d6e7a13d8b9864ec768a74f226f9326 Additional documentation for implicit private data collections
* b7463bef1da24a0bfab9342e098781c08276091e [FAB-18521] Replicate block metadata with block while OSN catching up (#2762)
* 90673b76d7829f7ea1c58de8da977173a9b50d8c Added a possibility to override chaincode.externalBuilders via env variable (#2643)
* 43ef319f90246bdd761ad5ddeac95ed2ef48e861 [FAB-18509] Stop panic of collection index path is wrong (#2726) (#2745)
* 6727a634592a298a2a29ef655d5613f674482778 Updated enrollUser function in write_first_app Doc (#2713)
* f0f16f492ebc0aed3f0dab06844faa5ca951a36c Update docs to clarify that an implicit collection can not have an index
* 98b65231530e4efbb6571084c92c5d4057782f00 docker network net_test -> fabric_test
* 56e2f8343af64ce8b80ad5267a47b2cc0764f472 Fixed grammatical errors
* ca1cf22b62859fc4e473fc789df00c51bb8b2c6d [Doc-Update] + What is a commercial paper section
* 5c5b7a5a5e254d94debe3dd8398b48ed83ac913d Fix a typo in CouchDB tutorial
* f424e95011b93d517e7af02b22120feb98d37c9d Fix typo
* c74cbb4259de02261724820a4dfab2ed9f34e174 Fix peerchaincode.md as well
* a089501b45c3482997aa9e395af8f7b0191aa048 Add explanation of `--ctor` JSON string
* f20421a6d3d11ef519840472440e548e6ef7de6a Clarify orderers seeing the transaction data
* 3f743a914e4f4c6b58f88260ae6395306815d516 Mandate TLS 1.2 or higher in fabhttp package
* f7eefeef6baa8e1ecb9e88c60ed7574054ff0e8d Clarify "identity expired" error messages (#2685) (#2686)
* f91d82fd16d91038190e8e0d1873f4366dd722bf Fix spelling mistakes in the Github Contributions page
* ef9b3f1caeaaaad0e737198a804e70ee00b39244 [FAB-18484] Return transaction forwarding result back to the client synchronously
* 981a4e89713bd2d4feb83994088ad266b9d10951 Link fixes detailed in FAB-18494
* a07a105e6e89fb49b5d562b0defcf7de92d5be68 Update ordererplan.md
* 6eccd4be70adfcd56ff6eea0a70d6bd3b193ec18 Added RetrieveBlockByNumber into blockledger (#2635) (#2657)
* de353c47064f91132d8c5a8d7659e14e4fbba6e7 Update peerchecklist.md (#2656)
* bd0c432cee47d160548c7489415c9dd70056fc63 Clarify doc for readset validations (#2647) (#2654)
* 47fee0976a7276a614d265afe8a4d2a169f4a72b Update secured_private_asset_transfer_tutorial.md
* 1c6b3a021644fa30dec25b63a92c2e282b5b7d93 Added single quotation marks to mask json path for jq command
* 9a47410d9ee384ce700b02e595c1fb739a6ec65e Update create_channel_test_net.md
* a172a69fea59a71e2306e6ba3be98ac0a93aa4bb [FAB-18479] Log error if orderer can't forward SubmitRequest to Raft leader
* 9750fc3e3365daede6cbf776cae4f445470ebbd2 fix duplicate entry in code snippet
* f7d216299446a5f8c508a3715c27af8db8d68dc8 add 'be'
* 6e787c7125f8813a6ebc230cb8cdb8fdb8e8726d Update deploy_chaincode.md
* 38f4713ed3189be56c6ab8c582e1290a80c2a7de Optionally disable gossip block forwarding (#2606)
* dc454fbe5de22c2702fc6110b6dfa43aa1f4219c Update docs/source/upgrade_to_newest_version.md
* d1cd43f84abd52aab5683b44274025207d0f1080 Govendor added to documentation
* 2c6e4031b3155e3b2ad4c2843d5218d1ef3db711 Improve error message for invalid consenter cert (#2587)
* 89c907e5a478b90f8934fc82b01bb477f52e9225 Removed early mentioning of organization R3
* 0022e8fd8f9253bf81c884fb7f7567e34f357546 v2.3.2 release commit
* 248a2206121f87551359d109d62adeb4e29d688c Improve snapshot dir error message (#2530)
* 25f6612dc37a0e227ba32d0dabba4639b348c856 Document ledger.snapshots.rootDir
* ce161777d33d37d24f7b7b91af3436a9ac3c6ede Cherry pick removing duplicate word (#2524)
* 5de1d022e26413445252cf6889845bf9ed5898dc Add Security Model topic to docs
* 13ef1e153c48053f9c74a021ff64c6c0959ac987 Fix link in `international_languages.md`
* b2c8d23f77a22fa86980d6f1b0087ac11193456b Fix old or incorrect contents in the doc build instruction
* f2462435b27f03f66940844d5be136e9b46d4dc8 integration: PKCS#11 SKI to CKA_ID mapping test
* 871d325d6aaf1743d364cb147724b4a0e7d05375 pkcs11: Add SKI to CKA_ID mapping for BCCSP [ #11 ]
* 0fb8e5a2ac7d742b1eb0e8c2d8f22748b5df4bc3 This commit upgrades goleveldb. This upgraded version includes a fix for [ #2463 ]
* 70c1d11b674ad4f9f2bda90cdcc9e74f9fff3c49 Fix images in network concept and upload new diagrams power point
* 2e9e732dabb6ed11084112cfdfbf16703ad99104 Prepare for next release v2.3.2
* fd84e78b54983a6f83d8fb9880fec29606df9355 Fix bug in snapshot request submission
* 90db11d3d5abf1d08cd864c392014e0386bc24a4 Report correct reason of stream abort in orderer cluster
* 1524fc9b6088661127dc8762e87fb0884ff3af98 Log stream total lifetime
* 8543389553ae22f84597520e983c7c0db85f0d5b corrected organization labels
* c61883e89270038d8ad3ffa271d2e91305af411f corrected Org1 text in Org2 box to Org2
* b156d91f0d6693bfa3e581f9c69e43e6ba67548a Update build to use Go 1.15
* c4d4f795d19a13eef0984f052342b8121fdaade1 Implement legacy name constraints verification
* a873a870c857f65aa4e91b05477e0204919a4b45 Add test to assert on name constraint behavior
* 230aa0e75af0d05f4eaf4615273d849601915472 deps: bump github.com/pkg/errors
* 15e3f94d36fd73144cdf9cc8c8d5702724e79775 Re-encode ECDSA CRL signature during MSP setup
* 4e91e45e1c73cab08dd01915fd751e41ad053aaa Add test to exercise signature validation change
* 8fb1a8109e1768f2536cba4e4b1284164c24b36d Adjust etcdraft error assertions for go 1.15
* 47b0bb64e36d13828c2eb6c29414c968aa4b5c9a Replace test cert fixtures with generated certs
* ce2cf2128794b59963d5e1bcf23ec579b57744a5 Set SKI, support multi hosts, add Signer to CA
* 932e0779f783be1a3f6f2dc2c3e344212ad0ee1d Fix typos in a "Developing Applications" doc
* d19dd3225609bcf5974df34ebf3fd17e2d8738c6 Update documentation to include Go SDK
* df59561c124b70149e9a3541fef76c8646687e0d Fix broken link in orderer deployment guide
* b2d6db64f929504f36d44a633f605b1271a797e7 Test network works with Docker Desktop version 2.5.0.1
* 1562d7ecacdf96946c4bf77f1f434f58e851d01b Update AZP Service Connection Name
* 7ad69c78ffe4a3bb5e96b16e4cbb04f35480aae6 Add Create a channel tutorial without a system channel and using test network
* 2f69b4222e9c9090b5c1ca235c1b59687566f13e Release commit for v2.3.1
* 17b7e4ff5c8ac8128c8c0a773f693550f972ddae Add peer log message for failure to invoke chaincode (#2339)
* fc63fcd1650b936864024193954bea0280459d1a Test network does not work with latest Docker
* 8dc9930bdea226d91b40e3189478ff592a0ffb9a Minor updates related to documentation for commands and more osnadmin updates (release-2.3) (#2322)
* c29420c55a09603b265161aeb48cea6e991f1695 Rename --channel-id to --channelID in osadmin
* 410ba71b4898f1ae3457c07d4d02e1a15f2811a9 Participation edits to network concept doc
* f682cadc2f9a759c3b5e7fbc14039b2073cba2ed Fix the issue of Nil/Zero-length-byte-array value (#2309)
* 23b677cff32ccdec0493065e1c3c14c6bf9015b1 Remove system channel from Test Network tutorial
* 1dc0b47982dca59f1a9df24a962b4e18743a2f14 [FAB-15648] document update: Non-TLS orderer with etcdraft usage (#1678)
* b144d49c1d2ce0c718439c54d873ca992c2be989 cherry pick test network doc chaincode deployment
* 7996176f2fa78fd6497fc734cd4887a0c4272f0a [FAB-18398] Added osnadmin binary to tools image (#2275)
* 7debdef0db6bf835d2316268d81d56519653044c Remove unreachable and unnecessary code in gossip membership (#2294)
* f99cff0ce6c5574b7a47b6e194aed3cfdd70f740 Orderer deployment tutorial update
* b4548dd5443241157785ac23f55509c0cfb2dd4a [doc] fix broken link
* a4a86d64b31521a3eae929440b9feee6886cc8eb Minor create channel doc typos
* c8d3e08bfbe1938dabb4da37886d9a5e73cffb56 Even more edits to docs for participation API (#2208) (#2281)
* 06866fb0340172066ca9a4adac7e021b970e6ad6 Revert "Minor create channel doc typos" backport
* e24a05e9bfe4593b50461d7b6c325a22bf07f6f8 Pass GO_TAGS to tools container (#2278)
* c2758ef135b33d430a8197747a825dc3a37ad5a1 Raft configuration doc issue after mergify backport (release-2.3)
* 157f5568070b8b128c034e3cd5eb495e15175f36 [FAB-18170] Endorsement policy page discusses NodeSDK
* f3cb99e5bc73358e73f457f6387d95ec7767a6b9 [FAB-18392] Clarify scope and limitations of test network
* d486efb599df7e9948c10610b30a1150c4959b0c [FAB-18252] Documentation should reference Java chaincode support
* 377290da547e8f31365a7a0e947727b27f81633b Remove anchor peers from configtx.yaml tutorial (#2257)
* e6b55b156900595a6b140b233a52a5bd11b17fa9 Update "add an org" tutorial to not use CLI
* cd578f37e636014a79cd2b43149efce54032351d Split command in "add an org to network" tutorial
* 0b2c7558737cc04bb46d1a0608aca58b8fa9ceca Add more details to logging specification examples
* 56a086145667247e9a13482f79c1dab1b28952e5 Minor create channel doc typos
* c8cc666b32abbdd557365baeef900e17baf6ceba Update image filter used by integration tests
* 4d213bafbebebf090919aae9c116539ed925c2f7 Add Language Argument to DeployCC Calls
* 9ab9368f6f0fb7141882e62f329fae7491170a1f Check correct error
* 06eb9b13e3e70de2d1c56af81bbfc3fd7f20a43c [FAB-18378] Log warning when peer is lagging behind and cannot catch up
* e5e858a302fbdd04f97746edcd9f7fd8dac82ad2 Fix unusual dash character in channel participation tutorial
* 5da3b0ff82ad83ca2da5d10059f5f2a3839d275e [FAB-17039] Skip retrieving pvtdata from transient store when txid is missing (#2183) (#2200)
* cc5a77c5ee84ee90060d5f34fa1f73eeb04865f2 More doc edits for system channel removal
* 0e774df4ae8e2468eb21ee955164f9b4dac989da Remove Short Names and Replace With Full Path in Fabric
* c91961c0c090d8bd6a6570e0a1e19803c9769eed Edits to orderer and capabilities concept for participation API
* eb22bbf85acebba5f4a83fc60fb5208a042efb95 [FAB-17954] Document CouchDB JSON determinism (#2187)
* b1fb856b3b27f421924a6e17881e0c70dc326585 Fix name of CHANNEL_CONFIG_BLOCK in the Channel participation API tutorial (#2186)
* bd491263bc58ab5932064ebc1bedaeb3928e4766 Update README.md to include link to Fabric v2.3 documentation
* 94fffbbcd03032e75ebce4d79358bd1ce1b5ffbc Orderer deploy guide edits for participation API (#2148)
* a455146c47dd2eaf4703fbd8ab0c996bb97e7d24 Fixes Hardened to Hardware
* 537ef5c15d5443a7b1adf62abfc8123ab303f09e remove repeated the
* 4c67ed31c19b97584d589861a5c5dcfd5f442807 update private-data sample instruction for Asset owner string
* ef8ff197cdd21167007f2d92a6c3aab2bcc443fa Remove reference to first-network
* ec81f3e74fa127fc504b1c2249b19ec421ea2a1d Release commit for v2.3.0 (#2144)

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=40697&view=logs).</details>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric/releases/tag/v2.3.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-09-09 06:43:58 +0000 UTC
    </span>
</div>

