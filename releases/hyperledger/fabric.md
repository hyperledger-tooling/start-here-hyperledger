---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div markdown="1">
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.3.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
v2.3.2
{: .label-grey }
            </td>
            <td>
                v2.3.2 Release Notes - April 23, 2021
=====================================

Improvements
------------

**peer and orderer - Implement legacy name constraints verification for Go 1.15**

These changes reproduce the Go 1.14 name constraint verification in the MSP.
Without these changes, certificate chains that would fail verification in Go 1.14 would
successfully validate in Go 1.15 due to the change mentioned in the [Go 1.15 release notes](https://golang.org/doc/go1.15#commonname).
Specifically, if a signing certificate contains a name constraint, the leaf certificate
does not include SAN extensions, and the leaf's common name looks like a host name,
then the additional verification is performed to ensure deterministic behavior relative
to prior Fabric releases.


Fixes
-----

**FAB-18427: orderer - Report correct reason of stream abort in orderer cluster**

This commit fixes a bug that makes the cluster communication infrastructure
always report an "aborted" reason after a stream terminates.

**FAB-18424: peer - Ledger snapshot request submission with special value "blockNumber 0"**

If a ledger snapshot request is submitted with the special value "blockNumber 0", peer is expected to translate the request to last committed block.
This patch fixes the issue where, it may happen sometimes that the request is translated to block number 1 instead of last committed block.
This leads to the situation where no snapshot gets generated, including any future snapshot requests.
If you have ever used this special value, we encourage you to check the list of pending snapshots requests with `peer snapshot listpending`.
If you notice one or more pending requests that are for the the block numbers lower than the latest committed block, cancel such requests with `peer snapshot cancelrequest` to enable the further snapshot requests to be processed.

**FAB-18304: peer and orderer - Fix leveldb manifest corruption**

This fix updates the version of goleveldb. The prior version of goleveldb had a bug which
could cause manifest corruption in crash scenarios, especially in disk full crash scenarios.
With a corrupted goleveldb database, the peer or orderer would fail to start with error
"panic: Error opening leveldb: leveldb: manifest corrupted".


Dependencies
------------
Fabric v2.3.2 has been tested with the following dependencies:
* Go 1.15.7
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
<details><summary><b>See More</b></summary>

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
* 2ff4e0e237d4288a6b687ac54eab5eb78248f1eb Clarify clientRootCAs guidance in core.yaml
* 4c4ddfc00227ff5d80ed9c6abc9137574f359682 Clarify clientRootCAs guidance in core.yaml and TLS docs (#2142)
* bc33cbb8c0802c5f637eebf2f143a449d830cd48 [FAB-18322] Check panic message in TestInitializeServerConfig (#2140)
* 504caaf2a8bf145a8c92067c4d0668dc230b596c What's New documentation for v2.3.0 (#2126)
* e7b81bace2f3e5ef55bfed07f4c11b618f43e663 Update core.yaml, orderer.yaml and docs for TLS (#2141)
* d5ed80d10d025914844de3f6d657a5819dc1b76e Add release note for RSA CA changes
* a09f0e79947de9c1b0c8cf754f311433d561fb0b Add integration test for MSPs with RSA CA certs
* 52f511dd4f740056c08cf1a1c61322c621692e02 Restore RSA support for x509 public key import
* c545195deb3f30d2f5c93bfca1ab135cfd77c307 Deploy production ordering service doc
* 5f2034f395eaf2df252f40fb77bfc15f20c26257 Add check for invalid key before hitting couchdb (#2133)
* 1f6fb0849c6cfb7be9818d40f1e40e35ff5c5a1d Chan.Part.API: Onboarding and follower CFT IT (#2094)
* 39a8545924e30c7339b9a9be9076b08f4dae3bb7 Fab-18337 Ch.Part.API: Test join system channel with app channels (#2128)
* ab55d501517e3092c394e3622025178e0fed8ac7 Add persistent volume note to peer deploy guide
* cb683e590bd2f89c76374152375791c9460ad222 Chan.Part.API: avoid flakiness after removing system channel (#2111)
* 48bf409d188ef56a6366d567d961e1a5129bf568 [FAB-18319] Ch.Part.API: IT Remove and rejoin channel from orderer (#2085)
* 70550076d5ea2b2454353af90203400a59fd3020 Nominate Will Lahti as Fabric Maintainer
* c17472808aa5b546c6eaa20d79b93371b3342a77 [FAB-18179] Channel Participation API Tutorial
* c08c5e3ba5cbffb1e5ff2a63d3a85bc3df94ff8e Update v2.3.0 release notes
* 09c0d75d3e6bd99dc85e5a01a1f2649e1a7d4be8 Revert "[FAB-18179] Channel Participation API tutorial"
* 40e845b6e122aa4bdb86fd76305ea4c6fd047df2 [FAB-18179] Channel Participation API tutorial
* 1f59e41a7916f29c3c3474ec706f321b894ff48c Remove unused type (#2120)
* d997115e85df0f8df846290065ebf4c54d9b695d Update Contribution guide to point to RFC process
* 01bfbba665d0ae3e1c6863803e170ea5570ff32e Update Go to 1.14.12
* 4a7efe9cf8de2f198efad447ddfd39819bcb4025 Remove custom errors from pvtdata store
* 5dcdf814ccb4c2ce870998699f4f15e8022b79f4 Remove custom error types from txmgr package
* 24868e956881c604d7dc1b561ce3f18ce2fc62b5 Remove custom error types (#2110)
* cd99b4e725ceefc8afa7a57608fbf8e0acacc770 Enforce Admin.TLS.ClientAuthRequired in orderer config (#2107)
* a01cda4a39d21ceca8c8495d83fecf6bfa631fc4 Allow osnadmin to connect without TLS (#2106)
* 7f6b5dd6cfa74ea0942e83f90b67274b87b8ff0e [FAB-18315] Ch.Part.API: Add remove failure metric for chain status (#2108)
* b9a8338a710e9590bbeac10313dbeebbaf62638c Add snapshots to peer deploy checklist (#2109)
* 4f1e0931eb233b82c0a53658bbba8a9debf61d2b kvledger/test for snapshot generation and bootstrap
* e5ebb7b8f8b3695f674b4d44864986dcb5524872 Remove the temp folder on error during snapshot generation (#2104)
* 941f0afba538c83feb6b254f7ed21226e49f3b74 Document additional snapshot considerations
* f1058a802cd6070ecb3e0aaf17793b8655940f70 [FAB-18333] Fix panic in cluster/comm#TestRenewCertificates
* 4e7201b679196d8c7ab171091a1219ef6ce7f310 Revert "Allow BCCSP config to be set using env var (#1900)" (#2093)
* b8f76aee33bb4feef54ce99f771d42532b416c8b Remove Jira screenshots (#2103)
* ca26271ec4b865287983444b42087cfec21175ef Redirect integration test logs to GinkgoWriter
* cd623d729936e83a7b0ed48440573b725c79c60e Update Jira instructions in contributing guide
* 01394c763439568f1078bea4ff56199bd2e571a5 Chan.Part.API: Rename pendingops/joinblock to pendingops/join
* 45afdbde4556b431af4982b3765a31b37d462768 Update channel_update_tutorial.rst with joinbysnapshot
* 421dddf9d77f53691bf27328fa452342026ff572 Remove unimplemented funcitons
* c590e372bc89b573cf8d6a7378488470edf2184d Prevent race that occurs after test timeout
* 901fe6ceccf0d85ed25cc62ad32a3fd65131800f [FAB-18329] Fix data race in cluster/comm_test#TestRenewCertificates (#2089)
* 73853ef640ad7fa4012c2d3cc5adb40974324b51 Chan.Part.API: join system channel using config block IT (#2082)
* 1e90c8889448c79e402f06c84106c0ca89bbe731 osnadmin command reference (#2077)
* 4b134cf2244d6a46d627c0e0e649254743377dbe Chan.Part.API: Rename cluster relation to consensus relation (#2086)
* d54ed923dc0fcf8ee72422e9f085d17e003b3dc9 Chan.Part.API: channel participation relation/status metrics (#2025)
* cc77194a342f156d329ebb65b756716525909057 Ch.Part.API: Allow retry of failed removals (#2083)
* 1f372da73f2cade0cbd1b7fcbaec9dc294269cd9 [FAB-18318] IT: verify DUPLICATE_TXID error when resubmitting old tx on a peer bootstrapped from snapshot (#2084)
* 6a56a0644e3ce61204081b4dd0990ee5afbbb6c1 Update configtxgen log messages for app chan genesis block (#2076)
* 7f6ead93fae5a06142ed43505d1f1306f26c0797 [FAB-18132] Ch.Part.API: Remove ledger resources asynchronously (#2027)
* 17f075c3dbee16a3dc2de48ca3efd1c43802c5c5 Add function TxIDExists and use in validation path
* d620ab33e9009c5e9f1ad03edab4bc9129f486ce [FAB-18298] Default cluster cert and key
* 636c36123f98433a9d250ad6dfca1c44d998eff1 Rename cluster relation member to consenter (#2079)
* 348e2c7ff433e88a02975c9071446c7c28325d00 Add default snapshot directory to core.yaml (#2068)
* 4db7e4cab557b200d8404d359fd8d3dac835876d Add osnadmin to Makefile
* 2b1b989163946a0e4f1b1388fb85e585015be689 [FAB-18290] Add channel name to pvtdata reconciler log msgs
* c15e44e3cbfd8ff59fa087de68675c164984e282 Minor refactoring
* a37ea5c300b2eeb1f6fb53c54f80000f23a4f030 Minor Refactoring
* bf57390ed331a7234a46609689a16b63c8966fd3 Optimize importing snapshot data into pvtdatastore
* 596f72088659486f7e44a8f690ab9e7c6b136325 [FAB-18307] IT: set deprioritizedDataReconcilerInterval to prevent CI flake (#2070)
* 32da54c9404a44bb71a088eff146c52aea6751d6 [FAB-17953] IT: add tests to verify channel config can be retrieved on a peer bootstrapped from snapshot (#2064)
* 91af91845a1e4bafc2ecb7efbe0aa3ffa34ae0aa IT: Add ACL test for snapshot related CLI cmds (#2061)
* ea81d212cb51109a517bdf9ee2c00e2f5aaa30eb osnadmin CLI (#1907)
* d7b1ed157670d6b1a2f3cc0b3e4e27908e4f2bcd Chan.Part.API: config-tracker IT flake fix
* b106d05f3e599fc377e80e8be1796266ed604f4a Updated comment for channel participation API
* 0d4c878bdad080bf864433e8d70eae8bdfdb3bca Fix link in snapshot doc
* 86200906660e5fd46df9b5148255b818706e6cf9 Use -c instead of -C for channelID in snapshot cli cmds
* 0edadacb247bf241f34d4b3af25ed2202ad5fb9c Peer snapshot documentation
* fac5bd1781b53ed21d2e23d831a673b63ac25ded [FAB-17953] IT: verify pvtdata reconciliation when bootstrapping by snapshot (#2052)
* 46cdc036771039d38b2a9c615e6edf62d6d85833 [FAB-17800] Update peer node command doc
* 2bf53e6235061b334b6b782d2da312b1c4c2ac50 FAB-18291 Ch.Part.API: BlockPuller that can be stopped (#2050)
* 067f09bb5720431986110e61b4db8f7366517221 FAB-18301 Registrar.JoinChannel takes the wrong lock type (#2058)
* e4c54fafddb1cdd1befd10a2216da0ba3b6c86d0 Chan.Part.API: config-tracker IT
* 275b545b52491ccac0c593557e50082bc042cbc8 [FAB-17800] Update reset/rollback/rebuild/upgrade_dbs cmd descriptions for snapshot
* dd224783b581d2b0224b0d232d75f2fb02434aa2 Add function GetChannelConfig in cscc and use in peer client
* 8758bde8d91eb10e6c8cf95975ee4013ecaec791 Update fabric-protos-go dependency (#2057)
* dedcf42e4242fc3164b57b722ca59a50f7104dac Add doc files for peer snapshot commands
* cf678beaf7a5e6c70dfd06d60ae5707cb2f8a715 Cleanup system channel w/ genesis block IT (#2055)
* 8899f5a59af2725aa2a4f39275f3b83cdf645f6c Avoid duplicated follower chain.Halt()
* 286293a29a7737f0ef7c2af29905010e0017b78f s/assert/require in orderer/common/follower UT
* a216637826d7bdc1754373ea078736225816674c check if desired version of samples exists
* 0d4e6ed22aac3b126f395aee79af11f1711982c5 Fix CouchDB tutorial queries
* c9439d8572a4f4dd218fdd4c10ed38b2deb34155 [FAB-18130] Chan.Part.API: Creating the system channel with a genesis block, so no onboarding is
* 2198c097ff69076dabcb0135ecdf55c246b3baeb Minor refactor/log change for orderer startup
* 62a8808b8dae510f4618eac9c3deeb8631bb59ae Rename channel particicpation CFT filerepo directory to pendingops
* 8f7e37a7ddeedde06b7207459787571cf68e487d Chan.Part.API: IT cleanup/improvements
* 44caec4a6a87df384644a5446eae583c87d78d0a nwo.GetConfigBlock retry until success
* 687f58d64e19c8216b7c9b5a92f78e19ab38cf9f Refactor and export pvtdata test funcs for marbles_private chaincode (#2048)
* b810925aa6946afd0a95349e4b1a8cf9f856a628 FAB-18283 Ch.Part.API: StatusReport on evicted etcdraft.Chain (#2049)
* 2c921bca2e793be53cbdcb786b97dce148ec5352 Return errors in rollback/rebuild commands when using snapshots
* a143ea9b9c422d38a7fb068b5800271848d8290c Minor update to joinbysnapshot cmd response msg
* d59af2c0090d80cfafe228de80c20595c8947154 Expose new Admin endpoint on orderer for the channel participation API (#1939)
* 60b5053814e0fdda8a41f0220ba9b3ba4b28e044 Update location of snapshots folder in IT
* e071f57bb123e8b80631ba9841c1b065edb6e0c7 [FAB-17953] Add integration tests for snapshot feature (leveldb and couchdb, no pvtdata)
* 105aeebed80b468763551c5f9c096b8f3286fb31 Make snapshots folder directly under <peer.fileSystemPath>
* 44f6ef5dd78c3fc7955f58f29b25021db2e6ed6a Pass channel config to service discovery
* 90733a0c28e1304542b58b0040aee732508b3d8f Log TLS handshake duration (#2032)
* 7b2b9f058447bad6225a0775236f9ab0bedf06fd [FAB-18082] Make RemoveChannel crash fault tolerant (#1952)
* 91886f635706703782092f929d3f91955ff18763 FAB-18108 Ch.Part.API: simplify follower.Chain flow control (#2026)
* d0eb424dc959d65dfad9b0f209ff0abd6fc3d631 Update tests to use CouchDB 3.1.1
* 48d532fd798270da7468ac1092aa999ed6f7775e Deduplicate orderer server TLS root CAs (#2029)
* 3c57d11743ca1fef6018b11c69ac667f204eed93 Copy Into Correct Slice To Ensure Keystore Password is Set
* c6f07dd89801694ab12148143a3c9d4eb25744ce FAB-18276 Ch.Part.API: extractSystemChannel must skip empty ledger (#2023)
* 69bc7319115545e8bae67877dcd8d4de5c87bda4 Remove common name from private data doc
* 0ae1f5a30624be6ee392edb30cf62d466777ce6c FAB-18198 Ch.Part.API: Restructure registrar init (#2015)
* 56118d0d93be37d6d4d3961e57516f1d76f8cad8 IT - update MSP and consenters set in single config update
* da83764ff61b92d75c69a4bc32ea7728aa379ff4 Update Nikhil Gupta's email address in maintainer file
* d43e5ddd5530d1e675fb9a5931e2d722bf92af91 Add stringer for channelID type (#2016)
* 0ee329582aee3ea0a78859be1a12b9300a9763bf Persist complete collection in the private blockstore (#2010)
* 4e2ac6f8a5d4913ed5526f21477ff7464049a8a9 [FAB-18270] Disable debug of CouchDB response body
* 192b03bad0ad1d285ee8a201ecb146a44401c651 [FAB-17800] Reset/Rollback returns error if a channel was bootstrapped from a snapshot (#1990)
* 9d02571a9ea6ac2f480ad13696dcc0fb73e7bd1f Fix bug in consenter cert validation logic
* 330dc724906217fa15e738ad60b6b2c5ca6cab89 Chan.Part.API: test member to follower transition
* ecf0bb75abd662d62356331f210a85ac4cda0b43 Miscellaneous channel participation IT cleanup
* b0a72913ce0ee01b118e1bc9a0d6068befe04199 Peer deployment guide
* 02ff2a30c95067ac961577a6becdd930b114c07f UT improvements for common/blockledger/fileledger (#1998)
* 9adde2e7d30e1cb8778f8dbb564e08bc49afb70d Update help text in test net tutorial
* e6fcef5430127ca966df79ced1dec771fb7973af Update release docs
* 60fa282709188bd7f72480e9a13f9e722bb0f956 Fix Node OU error message
* 114f03080632bfc77ab190add3335362d8bc00c6 Shutdown blockstore (if open) before dropping ledger (#1992)
* f79abaa110fc6d6d6089b183ce62333afb5a6368 Add Troubleshooting topic to Test Network for Docker Desktop setting
* 8c684eb3ad3e1a33f62d98226fe614febeecab4a Avoid panic when re-attempting system channel removal
* 49dbea4ffc68e32eef43e35b8a5c77b5e1280bd2 Allow tick interval override via orderer.yaml (#1981)
* 3f93c1766e8de7121df4bba677644e9fdbe45223 Improve consistency with channel participation errors (#1974)
* 4b1e6b782561b8cd2a4dc7c985d260d585548531 Fix chaincode lifecycle tutorial invoke
* f5201e933744198f9344c4b5e9f54d36d6e66786 Minor Fix - Add channelID in snapshot mgmt logs
* 568e08c33bf937cc2e6ca11392490a659c2f7eb1 Private data edits
* 99d71824c6f587959eb1071a26dfb96b17b87da4 Always Finalize the PKCS11 FindObject Operation
* 335de61adc156b7633cfb9536908bfb545488ff1 Add high level logging for snapshot generation and bootstrap from a snapshot
* 9ab2d38ce8e288c22e8b7a6975e88d1fb7dccd04 Couchdb indexes during bootstrap from a sanpshot  for legacy chaincodes
* 5455e2f8ac16807c6d91532df27f6a85d0142c57 [FAB-18111] Add docs for DevMode using new lifecycle
* 886d3cc5580e5059df587be49a35d5c374a08fe7 FAB-18192 Fixed TLS certs validation for consenters. (#1888)
* e904f0ec8bb6dd1bbd1c77e433f787179570feb5 Fix table width issue
* e264d1b2d7aa613013281c0c07e29367aeb972a3 FAB-18244 single node catches up with snapshot (#1964)
* f4a612c85331d1ca77592ea762bef5390b7645f7 Corrected to capitalized function names.
* 37b2bff4b8e449ef9f112d89555f845144cb1f4e Validate pvt-data during reconciliation for bootstrapped ledger (#1947)
* 4afc136de48efd9d4ade415c937a71531484f859 [FAB-18235] Properly handle Newest when a peer is bootstrapped from a snapshot (#1936)
* 0a9f7663a3a548385f3e4fa55e147b6dbce055d4 Allow BCCSP config to be set using env var (#1900)
* fa0213f146df6421cbd8a02e1751ea4cd2210e72 [FAB-18127] Chan.Part.API IT: Join as follower (#1861)
* 20eb85263a93436970ddfde2a8f22c3a70ddb180 Updates in master for v2.2.1 release
* 39353786dfa49b589a4cc7f9dc8130a7802b5361 Add two and three digit publishing
* fb3ad730ec67ac757fa37abb6815a4a055409032 Discover CLI fails fast when given inappropriate certificate file
* 79a4e01e58fb5f9a4205fef525d7775ed2219365 Fix orderer/common/multichannel flake when removing channel
* 03375dc50314e2fc96052ff66e8f01014d8ba306 Fix TestKeyCache
* a288fe4242ef1b9c1e25ab4bf82ba63bd6b72521 [FAB-18250] Check Error Before Returning Session to Pool
* fc0c3e252ff71981c3beb297176af632c86b85a5 Chan.Part.API: Int test for forbidden join actions
* d52a9e870478edf10729f660b776b344706afa49 Chan.Part.API: Int tests for forbidden actions w/ system channel
* 5f09b3bba5d05d01169fa24589e45d9d07771a50 Private data tutorial edits
* 69bd5cfcc5f26b2d52c8c25bb001e1b03742a403 Remove escc and vscc from list of system chaincodes
* a11fa5fb27161d0940a60524bda5620821ae17e2 Enable pvtdata store to receive pvtdata hashes during bootstrap (#1927)
* 356bf04f1944428660ffa36553d67bf4cee56d01 Fix empty address in peer CLI ClientWait log
* 1eec8430d7b83db21b99d6fd7ec1a6160a94c916 Remove GetSessionInfo Call
* bf5917fb821223e3745556d90c99db7070128abc [FAB-18234] Add joinbysnapshotstatus CLI command (#1910)
* d083849517bb08bb9e877b9ef091d6bfdf9553d2 [FAB-17691] Add BootstrappingSnapshotInfo to BlockchainInfo (#1922)
* 646260eb9e65c522bc2cd2e6bc0ec94e7e3eccdf Bug Fix: Saving big payloads by cache CouchDB (#1909)
* 3a8440de792b95487bb433820ce652a9da4e4b55 Fix flakey raft/cft integration test (#1916)
* 5152bead1e81ff2a8d6d833f6772cdf1f96ba5fa [FAB-18234] Update fabric-protos-go dependency (#1919)
* 5bcb5e0b0884e05e2aebf19fe7f349dd98a72ce0 Implement interface SnapshotPvtdataHashesConsumer for pvtdata store (#1908)
* e801c2f7c0e9d895141a157a06dcd4a4b5b5132f [FAB-17691] Update fabric-protos-go dependency (#1914)
* d76553aa683da626051e8a451b200eb695abb7bb [FAB-18237] always update stateInfo message upon chaincode update
* bbc5f5f458611d83ecb5c83e29e1a702ee6d6873 [FAB-18164] Change CreateLedgerFromSnapshot to async (#1889)
* 17858a570ebd0c783e1cb25a4f5ffe2e7889653f Update 'Using Private Data in Fabric' tutorial
* d67feb1e478f477d9d8572ee9b47d63111ef151a Bugfix in collection config history mgr
* b89e02b20806018d27bd6d75c86c12ad8f602249 [FAB-18235] Update fabric-protos-go dependency (#1899)
* 379f6f023ebbc63b972d6559df521f329eb83cce Clarify tlsHandshakeTimeShift CLI help text (#1896)
* 39601e2c594089613924df4edfbbf9d20f807e5e Update write_first_app.rst
* 5a372b9c0ca17707c50f2bb9436f7494021924ea Correct the explanation for signcerts in Membership section
* 6bf0542edb5bc87f2da4a9d7dee1c19f8a48e311 address review comments (#1890)
* ebfd084fedb262393ec5e004990d8dedc51e6cc3 FAB-17911 Ch.Part.API: join system channel (#1884)
* 91f08660a6364b6ad13052a8d447b9d969a26947 pass unreconciled data to the pvtstore commit
* de6c1fa502e7c213dc0dce4d3ab544b136daf960 minor refactoring of missing pvtdata retrieval test
* fd8559f5a86897e44565ab1268472e2f3ffbd46a add config for deprioritized missing data access interval

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=33614&view=logs).</details>
            </td>
        </tr>
    </table>
[View on GitHub](https://github.com/hyperledger/fabric/releases/tag/v2.3.2){: .btn }
    <span class="right-align">
        Created At 2021-04-23 20:25:15 +0000 UTC
    </span>
</div>

<div markdown="1">
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.2.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
v2.2.3
{: .label-grey }
            </td>
            <td>
                v2.2.3 Release Notes - April 23, 2021
=====================================

Improvements
------------

**peer and orderer - Implement legacy name constraints verification for Go 1.15**

These changes reproduce the Go 1.14 name constraint verification in the MSP.
Without these changes, certificate chains that would fail verification in Go 1.14 would
successfully validate in Go 1.15 due to the change mentioned in the [Go 1.15 release notes](https://golang.org/doc/go1.15#commonname).
Specifically, if a signing certificate contains a name constraint, the leaf certificate
does not include SAN extensions, and the leaf's common name looks like a host name,
then the additional verification is performed to ensure deterministic behavior relative
to prior Fabric releases.


Fixes
-----

**FAB-18427: orderer - Report correct reason of stream abort in orderer cluster**

This commit fixes a bug that makes the cluster communication infrastructure
always report an "aborted" reason after a stream terminates.

**FAB-18304: peer and orderer - Fix leveldb manifest corruption**

This fix updates the version of goleveldb. The prior version of goleveldb had a bug which
could cause manifest corruption in crash scenarios, especially in disk full crash scenarios.
With a corrupted goleveldb database, the peer or orderer would fail to start with error
"panic: Error opening leveldb: leveldb: manifest corrupted".


Dependencies
------------
Fabric v2.2.3 has been tested with the following dependencies:
* Go 1.15.7
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
<details><summary><b>See More</b></summary>

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
* c44e603d18819adb562b4a320c5e7569761ea244 Remove BYFN
* da4f52fe74bbe8a02725dd55d19d60e5ac9680d4 Remove BYFN from the toc
* 19d79a4b0a61e7a90e9b7bba6489832f6424f7da [FAB-18034] Fixed FabCar docs formatting.
* 3ee83a7b79ddf66154f428b0c7101ca38e458763 [FAB-18034] Improve FabCar docs , Fix queryAllCars description
* f743289b99d9957ebfff4886d921917d08c05322 [FAB-18034] Improve FabCar docs with better context, Fix queryAllCars description
* b99f6aee6760ca0c59ea96bb64a02e488c1efb2b Eliminate warnings when building documents
* f0285ca758799c36d6a3642204f64d334cb9b189 DOC fixed broken hyperlinks fabric doc, updated old output in go.mod
* 580f90a46893dbe9abec5649b3a96c1cb5e028e2 [FAB-16435] Improve gossip defaults - disable state transfer (#1478)
* ec42cbd0d1a5c0a1d46138743be214eb773fb213 [FAB-16435] Improve defaults - maxBlockCountToStore & blockBufferSize (#1477)
* 325b762102d970b135bb794a541e8453eb54d64a import collection configs from snapshot (#1460)
* 327765d59a9dd095e0282eda18c8e6306594daf1 Remove DocBuild Job From CI
* c222790d489107163ec7b398f15b17b4a94b3551 [FAB-16435] Improve gossip defaults - Peers to be leaders by default
* dd13262fde8ee9aa7f910d9dc986ec43d097d63d [FAB-18030] Discover all peers first before testing gossip membership to avoid flakes
* 09de0b86b19427754f755ee12abbda739fa224da Fix unsupported syntax for policy in the documents
* bc3c63e06582dcc7647dd0ff8e50af3ec20b79ef check iter error (#1468)
* 701bf56b4e654a2a9bf6b264dfc41cd7816bf503 [FAB-16789] per PR feedback, fixed sentence about peer pulling block from orderer on joining channel
* 34cea91372246076c5d7b6df58dd58c93518f64b check leveldb iterator error (#1428)
* 68f68ca3bed4f66891c8264a725645bb60e08300 Revert "rm old proto related code from transient store (#1464)" (#1467)
* c71209052cf5075af7457725f05aaa0028b56d57 rm old proto related code from transient store (#1464)
* 02f056946835d1847942b650ff16e2325ebb676e [FAB-17992] Remove ledger blockstore data for a channel (#1423)
* ef97677e893357f456ab42f3f1b0940c0641cce4 Update configtx library dependency to v0.0.5
* a9d25f05ce098692e9c859ca20d2bd4807644a37 Remove references to blacklist and whitelist
* 3e29ecd4f5644feaf3574add437edf6432e8d9ae Fix logging of recovered in NewPublicNymFromBytes
* 52436d3f6ae9bce76366301a3639368d59ce94fe rm interface from confighistory store
* afc272014ccf3b4817e1ee891d0c8c683e041ff6 Remove whitelist comment from core.yaml
* d91de163de991932bdf970dfbb3b1bc11b2726fa [FAB-16789] per PR feedback, fixed sentence about peer pulling block from orderer on joining channel
* c59d45e47afa7b237fef08b2c032a787555bb2e9 [FAB-16789] removed sentence about P1 peer using orderer, per PR comment.
* 067044225cf58edd009839dee8675164278380a7 [FAB-16789] Fix peer join description in network key concept
* d728cd69c26351b60c63bb311397faa880e36991 Restore assertions related to peer address config
* 193a7de881cea632c533c8b4b1fa03748ff974aa [FAB-17539] Always remember anchor peers in membership (#1422)
* 65345cfb0fbeeb768a6fb85a82db6ad3e993d613 Explicitly set gossip.endpoint in integration test (#1455)
* f29b7f132071914b466a39a2aa21da2b811f74be validation (occ) pkg -- consistently use testify/require (#1454)
* 2b408a611b4436a28e8b8a53db694607d7f6e66b txmgr pkg -- consistently use testify/require (#1453)
* fb9750555ea3946c9c03019a39c51d8f189af495 statecouchdb pkg -- consistently use testify/require (#1449)
* 5f098ec41b2fd1fd3fb9fe4fa522c3925ac5fc4f statedb pkg -- consistently use testify/require (#1450)
* 98f1858505508d1cf9dfd0b0aa6cdfbec6092ad6 rwsetutil pkg -- consistently use testify/require (#1452)
* 2188ebac363e08dfa80c5cb25755c250f6f13f7d queryutil pkg -- consistently use testify/require (#1451)
* 65e88bc904eb5253c32b00ae6bd706db2fe2368b [FAB-18021] Improve log messages in `msp/configbuilder.go`
* 841e7f033b0cac34e74ed8c38824f7bd63fa9d23 ledgermgmt pkg -- consistently use testify/require (#1445)
* 341fa8c3e1f387fb4a78988ad2dd72aba1fd398f privacyenabledstate pkg -- consistently use testify/require (#1447)
* 8f7cef399bcf51e5a9bb13bfe3bbfa5b91f2ec47 cceventmgmt pkg -- consistently use testify/require (#1443)
* 9f18781576b9ca3ff533c8a65b60fa6026c78369 confighistory pkg -- consistently use testify/require (#1444)
* def99d1960daf1843cd77d65071bd19b99294fcb pvtstatepurgemgmt pkg -- consistently use testify/require (#1448)
* fe7fd6c586f5b0bd5953135cb98d8f40a7949307 pvtdatapolicy pkg -- consistently use testify/require (#1446)
* 833438fb1bf812033351cd232917c11cb17a34cb kvledger pkg -- consistently use testify/require (#1440)
* 0c679551ca1efb8bcd90519fc18ed5f383e559ca pvtstore pkg -- consistently use testify/require (#1439)
* d74a1162fd64369af6f8e7680e58dd5e6926b26d stateleveldb pkg -- consistently use testify/require (#1438)
* 7548f29b486a7e2a6de04649e49bbc862ce6bed9 replace testify/assert with testify/require (#1437)
* 87409f0d5a9fb5f82e2fd56a9277d6deabaf2943 Remove call to couchdb API _ensure_full_commit (#1435)

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=33612&view=logs).</details>
            </td>
        </tr>
    </table>
[View on GitHub](https://github.com/hyperledger/fabric/releases/tag/v2.2.3){: .btn }
    <span class="right-align">
        Created At 2021-04-23 20:23:21 +0000 UTC
    </span>
</div>

<div markdown="1">
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.4.12
                </b>
            </td>
        </tr>
        <tr>
            <td>
v1.4.12
{: .label-grey }
            </td>
            <td>
                v1.4.12 Release Notes - April 23, 2021
======================================

Fixes
-----

**FAB-18304: peer and orderer - Fix leveldb manifest corruption**

This fix updates the version of goleveldb. The prior version of goleveldb had a bug which
could cause manifest corruption in crash scenarios, especially in disk full crash scenarios.
With a corrupted goleveldb database, the peer or orderer would fail to start with error
"panic: Error opening leveldb: leveldb: manifest corrupted".


Dependencies
------------
Fabric v1.4.12 has been tested with the following dependencies:
* Go 1.14.12
* Fabric baseimage 0.4.22
* CouchDB v2.3.1


Changes, Known Issues, and Workarounds
--------------------------------------

**FAB-12134: Same chaincode source receiving fingerprint mismatch error** -
Chaincode installed in different ways may result in "chaincode fingerprint
mismatch data mismatch" error upon instantiation. This may happen when
installing chaincode by using different SDKs. To workaround the problem,
package the chaincode prior to installation and instantiation, by using
the "peer chaincode package" command.


Known Vulnerabilities
---------------------

**FAB-8664: Peer should detect and react when its org has been removed**
This is a relatively low severity problem, because it requires a significant
conspiracy of network admins, but it will be addressed in a future release.


Resolved Vulnerabilities
------------------------
None.


Deprecations (existing)
-----------------------
The following functions are deprecated and are targeted for removal in a future release.

**Support for automatically vendoring the chaincode shim into user chaincodes**

The fabric-ccenv image which is used to build chaincode, currently includes
the github.com/hyperledger/fabric/core/chaincode/shim ("shim") package.
This is convenient, as it provides the ability to package chaincode
without the need to include the "shim". However, this may cause issues in future
releases (and/or when trying to use packages which are included by the "shim").
In order to avoid any issues, users are advised to manually vendor the "shim"
package with their chaincode prior to using the peer CLI for packaging and/or
for installing chaincode.
Support removed in v2.0. For more details see FAB-5177.

**Support for CAR chaincode package format**

Support for packaging chaincode using the CAR format will be removed in
a future release.
Support removed in v2.0. For more details see FAB-14720.

**Support for invoking system chaincodes from user chaincodes.**

System chaincodes, for example QSCC, are intended to be invoked by
a client rather than by a user chaincode. Invoking from a user chaincode
may cause deadlocks.
Support removed in v2.0. For more details see FAB-15285.

**Support for user chaincodes to utilize the chaincode shim's logger via NewLogger()**

Chaincodes that used the shim's NewLogger() will need to shift to their own preferred
logging mechanism.
Support removed in v2.0. For more details see FAB-15366.

**Support for peer's Admin service**

The peer's Admin service exposes APIs such as GetLogSpec() and SetLogSpec().
Instead of using these services, utilize the HTTP operations service that was
introduced in v1.4.0.
Support removed in v2.0. For more details see FAB-15390.

**Support for specifying orderer endpoints at the global level in channel configuration.**

Utilize the new 'OrdererEndpoints' stanza within the channel configuration of
an organization instead.
For more details see FAB-7559.

**The 'Solo' consensus type is deprecated.**

With the introduction of Raft-based ordering service in v1.4.1, it is possible
to deploy a single-node (non-production) or multi-node
Raft-based ordering service with no external dependencies.
For single-node (non-production) ordering services, utilize Raft-based ordering
service with a single node instead of Solo ordering service.
For more details see FAB-15754.

**The 'Kafka' consensus type is deprecated**

The 'Raft' consensus type was introduced in v1.4.1 and has become the preferred
production consensus type. There is a documented and tested migration path from
Kafka to Raft, and existing users should migrate to the newer Raft consensus type.
For compatibility with existing deployments, Kafka is still supported,
but may be removed entirely in a future release.
Additionally, the fabric-kafka and fabric-zookeeper docker images are no longer updated, maintained, or published.

**fabric-couchdb docker image no longer updated, maintained, or published**

The fabric-couchdb docker image will no longer be updated, maintained, or published.
Users can utilize the official CouchDB docker image maintained by the Apache CouchDB project instead.


Change log
----------
For the full list of changes, refer to the release change log:
https://github.com/hyperledger/fabric/blob/release-1.4/CHANGELOG.md#v1412


## Changes:

* 56c2b126ef097635d2b72f753978c2fa027fb123 v1.4.12 release commit
* d276ee15f027eb72be2777f8ee13d2124bcc38f0 pkcs11: backport integration test to release-1.4
* c810dca48886d4f4ac99d598d0e591c3378fcfb4 This commit upgrades goleveldb. This upgraded version includes a fix for [ #2463 ]
* 16123fe63f9d365a653ff086954d3b79395fda65 Update Docker Publish Script
* 77facb430c1f001b612a608bc711ba9d324124e6 Release v1.4.11 commit
* b6822cb015bf94e3d686d2816565f075e0205791 Report correct reason of stream abort in orderer cluster
* 4db20918ff1b19d8f92ea5ffbf4311377567b47f Log stream total lifetime
* a7f2b157ba658a0d3a9c88ecd299d75ef8cb5607 deps: overrides to use go1.14 branches
* 999051da659256c808c56e3aae98d8e02b84ca3f Remvoe mockery from standard gotool targets
* f15b2b40e28f77acbe9a03bf20e5631222f44c8e Prepare for next release v1.4.11
<details><summary><b>See More</b></summary>

* 59d406acc5fae9ad5b96a4588b0aab298019db03 Update AZP Service Connection Name
* e3d4a0a9b0c0f0a8bda695d722b1669bd597bf19 Update image filter used by integration tests
* a7e659d87bc523f2ff8c3441b496618727034702 Pin npm to latest-6 for compatibility with node 8
* 7d1ee82acbdf7b7ef85dff6202b1e35464caa090 v1.4.10 release commit
* adfdd61bd0bfd86f9560821c452b3ae2663151bb Add v1.4.10 release notes
* 3813607c1468c1e825a2f7897e372d871d9fa51a Fix the issue of Nil/Zero-length-byte-array value (#2312)
* e95a134f171bae9c2af26d0f0fdfa5d06782003e Remove unreachable and unnecessary code in gossip membership (#2296)
* 51a3a52260f6228bdd57eb11cdf2a564c80c766d [FAB-17039] CherryPick: Skip retrieving pvtdata from transient store when txid is missing (bp #2183) (#2203)
* 746b7e9a3815a88c751d27d2c2871243e4370eb1 [FAB-18323] CherryPick: remove ephemeral from BCCSP SW options (#1553)
* 25d99ba5e79f4867367bdd444d7720e51ac8ae87 Update endorsementpolicies.md
* 70040009218a4123473e6b050044465573853876 Bump Go to 1.14.12
* 2dbf8d683213b20d67c24b97f32c9496c3439711 Bump version of golang.org/x/tools
* e876e6478ae81978d0b33fb73cb085a31beefcab [FAB-13370] increase go env timeout from 10s to 1m
* 1d7b8766fd85ecbce8e4decf75dbfd01c41d23ab Increase Eventually Timeout
* a25b63fd42b8b9e9a8b0f03da050757365de6062 Prepare for go 1.14 (#755)
* b5a12de28553481140374865850e1632cbb2b016 Log TLS hanshake duration
* 56d7b8429ce0286c27fd78205fc2887654e8c512 Deduplicate orderer server TLS root CAs (#2030)
* cf344b5ddb831eb08591242dd4b81519ce5daa82 FAB-18244 single node catches up with snapshot (#2022)
* 83c833c251337973baf32050ac42df3938c53460 [FAB-18270] Disable debug of CouchDB response body
* 75f9fe7f3d163f81e2a4f6db566ab47a7ed96cca [FAB-18265] Always Use DummyKeystore For PKCS11 BCCSP Provider
* a40f9d2779befb25b3d9a76cc2e132a12b95b8b5 Allow tick interval override via orderer.yaml
* db1abf695cc56d1f8a403c671be562e71a7c1648 Always Finalize the PKCS11 FindObject Operation (#1978)
* df50dea66e8375a2ca6f8e99665f4202e166592f Update devmode doc to note TLS must be disabled (release-1.4)
* 4af8308fb529281fa4c0e759dc3fb203930acdad Prepare for next release v1.4.10
* da55272a75e66da2c91befe89430dee8b9580df9 Release commit for v1.4.9
* 5146a9f5c52d59f0e5ff478194827fc3c65a930c Remove No Longer Relevant Release Note
* 4924294cc5e680e11a3f9766415dc943e6a97088 Update release notes with FAB-18250
* 56a81f798a3e1d8c445b65d57e47cbed887f2878 [FAB-18250] Check Error Before Returning Session to Pool (#1938)
* 17e171ba25e6acc22d8fed3a437a738a5f1a8f78 Remove escc and vscc from list of system chaincodes
* 2d63281adc0bdc76409d92ad90f015350ecbc870 Remove GetSessionInfo Call
* 4f1e3408802e567abba60e0bba02a96d7be1ec4e Add release notes for v1.4.9
* 40abeec3fe4243b625f6cea5882c46f8ebdc0854 [FAB-18237] always update stateInfo message upon chaincode update (#1915)
* 693cae5be282be51a48118ae4e8764e282b48cb8 Clarify tlsHandshakeTimeShift CLI help text (#1895)
* d9a8bc9ad95d44995968809cb4598a2dc74f0a4c Peer CLI communicate with orderers with expired TLS certs
* 51ffd55de8076d70397b169139fc0c9db6f4cf05 Add extra queryexecutor nil checks
* 95e4cfd3a5cea14148402573e59acd68d8792f05 [FAB-18208] Do not sign gossip message if membership is empty
* 5201e86feaad1221dc9de5ff8aea50151a4e78cb Fix data race in gossip/discovery test (#1865)
* 11cbae972e223b3545bc2e87d1842d055a95b908 Add object handle and key cache to bccsp/pkcs11 [ #11 ]
* d6261467ebbce1ea25db344bed82623050930865 Drain session pool before creating new sessions
* d0c506528c11ad4b7115ca6859fb39aea5acd13d Fix Broken Doc Reference
* d308fbf7cb90ee75342248b834c53fb9bab7a802 Re-enable Skipped PKCS11 Tests
* 80d3934494bdac9a4be8aec456c2b153161314ab Fix broken pkcs11 tests
* c8d124f87235df7085ff867254af95dd4bdd6cdf [FAB-18073] Add integration test for dev mode
* 9848841ad97db7db16cafcfeb40953bee364d62e [FAB-18171] Disregard certificate validity period in intra-orderer communication (#1825)
* 243dc0e1cf39d36609a9b5c8d4e8b54d74290d2c [FAB-17539] Always remember anchor peers in membership (#1422) (#1815)
* f208ffeb4dfda3f520ae5e481ebe0b58230addab [FAB-18188] Log orderer and peer cert expiration date upon startup (#1804)
* a19c9ec31c43148a30efec89806c183154d9519e Remove Latest Tag Publishing
* 8c85f7743f3711c5810b1fabb5ef36caea1f9e9c Fix and improve discovery TLS authentication comments in document
* dcba9b12284534f912ea2388f6c2066c888194f3 FAB-18163 TLS Timeshift w/o Separate Cluster Port (#1726)
* 4eaec1d4b77fafb31a777a86f7e7c27ad27df8fa Use correct gossip SecretEnvelope reference
* 6361bff7dc0d2f2c5ee2c5e66aa6ca7af319bee7 Update release-1.4 for Fabric CA v1.4.8 release
* d3c3aac7947d28d13759f01bb0022e9e1896cece Fix link in Develop apps doc
* a3486d376e8277205dda4a87231794da6aa52adc Prepare for Fabric v1.4.9 (#1627)
* 29e1e77ce9d7c7c65239939da74d0345fc99c038 Release commit for v1.4.8 (#1625)
* 112c6d952bf6ec5accf6763e6108f0976d4ec924 Add release notes for v1.4.8
* ae1395ba44065529b200cf688db18d8f338ca1ee Tag built docker images with BASE_VERSION and TWO_DIGIT_VERSION
* 81f32de36a775f8c1595a29a69550f2c2166a817 Fix latest tag on ccenv
* caf5b56b3ba8c56cc12e2fb47cf6904ee8c8b3fd Raft: Check suspect info once per suspect interval (#1602)
* 66349cc39b5af1e779898e74082620f5a73cf30c Print channel name in learnAnchorPeers
* a7eb1f7c1029beb9a93ec2bcc55c0059c113dbb6 [FAB-18043] Correct the code comments (#1530)
* 34294ad808a671fdf04c3bc72451073c652390da Only canonize ECDSA signatures in MSP:IsWellFormed (#1495)
* c2ea18f26dc2b09a5a9f0929508721e91ba1875f Bump Go to 1.13.12 and Third-Party Images to 0.4.21 (#1492)
* d34fd05c13bb61b9fb9c5a2635f926513ecf41a3 Fix wrong link sampleconfig
* 4a193ed5fc651a9b871732c72232289d7fca581f Set http header entries before writing header
* 9d2258c81d56dafe762679fdddb12e3e6cba8e21 Update gotools mockery path for release-1.4 (#1417)
* 65e735383f1c79c3787286cbc06c5f2b59bf3eda FAB-17161 improve error message
* 52ee9472399f4ec5e875ddee9b59c10d41cd1687 Fix the installed binary list in the document
* 877cadd9797ef7df16e0a415e802e0bb77476f3f [DocUpdate] configtxlator decode/common.ConfigUpdate
* 38b40b50496da0ac7d139c4bedb70ea2ae8e4c82 Prepare for Fabric v1.4.8 release
* e0afaa7415a8f11990ce2142bb1d6700d74e147c Release Fabric v1.4.7
* 51138b83da24b7b6651450c6c3c9ec260ef45624 Add release notes for v1.4.7
* a178051d430cfaac333c5c37dc3312cb90a2ed5a [FAB-17728] Add 100ms delay to pkcs11 create session loop (#1253)
* ea185b82628e283c82a87a2b13c3bcd4815a90cf Correct HSM environment variables
* 8ff5d1648971ae9e16815e9b4a1a83aba3de1b13 Bump baseimage version
* 6112b9967864847e8d20df6ab76adb06ff30020c [FAB-17821] fix: use keyword as variable name
* 1964a1bec260075ff4249865430e1ed76f64431c [FAB-17778] MSP.IsWellFormed: Only allow canonical CA signatures
* 506691955bd177996864c8ac2c40039b50c1f537 [FAB-17778] Force sanitized signatures be canonically built
* c66c3c4f4f474ed995066052faa5479c8b47ded5 add the sample policy to remove the test warning info
* e1db649b47394c182bd932d7895b9b5b9be7cb1a FAB-17552: add unit test for createKeyStore
* f27803fa77fbbf2f68d470aa515e7444750f20a9 FAB-17752: following review guide
* c40337482ec97d4fe053d47105710b90c3bfbb2d FAB-17752: return errors when creating keystore
* 2f740c4e67bc3160707d1b58685428e864652d4b [FAB-17732] Port HSM updates to release-1.4 branch (#1110)
* 1f0a0dd5316310d299a02f0588db3f7ec50c965e Validate session and get new if invalid
* b03b3d9fed8f4e962dbe1d52a3bdbdc8cc6c31f8 [FAB-17540] Fix for race read/write tlsconfig (#1050)
* 856f215b82fcd1a5f0349fba8768921b9d591c96 FAB-15461 Fix election adapter to return correct peers
* f9e80e808e9324441b196ca16b887ed7a69ebaa6 [FAB-16879] Add stack trace to couchdb http errors (#1048)
* c68ee5c9c44940fed92cc3ec6e3d784330ba0611 [FABB-148, FABB-149]
* 900773935d4df44e760f7e469b84646cad4c01c0 Properly handle malformed gossip envelopes (#1037)
* 780b16fcc9b0e714f7ae2615c90fec7b2eed9f22 Fix organizations typo
* 5c2a9969aa0d3c4d9892805de3b441dce2c6f19e Update to go 1.13
* 3b5b58b574a2ffca8912ced8ad792f3c64eb0865 Fix deadline logging test
* be925f8a117572d30aa075b419e2f4a799e20f19 [FAB-16810] comm test changes to support go 1.13
* 7cf38b5b8b684385f58c5aea00995437edda5fd9 [FAB-16810] bccsp test changes for go 1.13
* 9461ba23e99452e5a8751807fd452a34aa375dad [FAB-17696] Fixed Wiki Link to Contributor meetings
* 1e512255ea31b277cddc33cd925d6e3313d66505 [FAB-17109] Retrieve ReconnectBackoffThreshold as duration
* afbc42f5b768797947d02f8ec2f6e88b0d490da5 [FAB-16951] Alternative mechanisms to find pkcs11 key
* ca93be5566ca62cbc14586b8898fc417c1e46fc7 BCCSP initialization cleanup
* 2bb6415183457e355e36e4a68d0f6d8c8fbfe76a [FAB-17517] Only Initialize specified provider
* defb36c634626c9571bfcca6f31a023eadddd90a Add MSP Key concepts topic to release-1.4 branch
* 609ddf8ef338e86524b2603e4a00a903e9ed9d65 Prepare for fabric v1.4.7 release (#743)
* 635fa7bc8054ce75fd6af6fdb138be2c4e9996ba Update release notes for v1.4.6
* af2b4627cd27b1a2df94f14d0d93517fac007284 Release fabric v1.4.6
* 87df0516af1bb2cd7cf8b7d5eaa7b0b1d9ce1210 [FAB-17515] Support configuring BlockValidation policy for orderer group
* 29c58ac3ee18184da41fa198908229bcfa674f06 [FAB-17431] Decouple javaenv from Fabric version
* ac6305e2580e6362605c4745e600be7a8198272b [FAB-17523] Endorsing peer was not honoring RequiredPeerCount (#716) (#733)
* 0c421c8136f0ed0d263028c468ed61018332f947 Fix nil dereference in etcdraft config parsing (#724)
* 9072299684a6fb3e3c7bdf1e3b6fb6f92502d4b8 Add ending braces to ReadWrite set.
* a0b758412b3e76a0f4c56167a817a321924d53c0 Optimize inquire.IsSubset (#713)
* 60c8ab9127d8b5c38a1eae185912413182026efc Prepare for next fabric rel v1.4.6
* 11ff99170f1dc31aa6c657149b3337ec4fb22d73 Release fabric v1.4.5 (#695)
* 1893808704b077f92eefe83b739f4f56840476c2 Remove rollback code from private data store
* f354c818387dabd853cae0dfb0389c6370d88999 [FAB-17472] Clarify doc and samples for NodeOU Certificate
* d45bac4c8221191b8f424668fb1a51eebe794977 Add release notes for Fabric v1.4.5
* a9a1d07ab615e3fcbce4881491f7e07aa0da1035 [FAB-17059] Extend private data integration tests to cover case when a
* ca1ae38b19a531b37c62c030bd44616136b64c1e [FAB-17059] Change collection membership eligibility checks to
* e75bc716e8f4b501815324a4ee836026d59f4c41 [FAB-17479] Migrated Kafka cluster can be safely expanded later (#642)
* 5eaae3a9940d576e99b2202b243e56fc75eda070 Explicitly enumerate orderer and peer metrics
* 9faad9ea3e1a2868f319c4b7f9ca3c83e2df781e define couchDB connection pool size
* b27a7c7e6a1df2fe02b8030a2abccc5fc6df4cc8 [FAB-16681] Fix inconsistencies in the fabcar tutorial
* 46daf02f71019daea2c6ef17c3f7615f4fc51d86 [FAB-16508] Update commercial paper tutorial to match code
* 0a6993d69cef1c79a26adb30cebae3f41b81ef70 Add Documentation Maintainers to CODEOWNERS file
* 52e51550b0b8f08b2f3c9052e851a82c002d406f Point to Artifactory for chaintool downloads
* 1786f10f0cfc277c3e18a2f393a25ecfafdeb481 [FABCN-378] Update links to chaincode JSDoc
* bc3bb1af4931b1450fcc71fd5306c286153c00f6 [FAB-15578] Fix typos on the endorser metric name
* 975cc00addd49da9d1df4e318a7e55c3f5735c8d FAB-16033 Update channel_artifacts location in doc.
* cae8b5537916fcdac5752587ca2747ed4eda2cf7 Static leader should not give up retrieving blocks
* f0ea8256ad0b0d0f9de3c6473b81df85c4c6d33d [FAB-17169] Add AZP Status Badge (#511)
* 3ad450d47af9901e6ca178870c85205cbea42303 Go SDK link should point to 1.4 release [ #476 ]
* 1b6bea78aadba02df05094f8a3a4bb0af542e45f Update dead link to Go Chaincode SDK
* 9ec196bcc8db009018fe3aaee19993ebe21b47c2 Add CODEOWNERS group
* a8639bacd3e3516ee77fad3bdf00110710ae7cd9 Allow seperate TLS config for cluster and client (#393)
* d4dca959fb76dd59db5bda2c2db8d4b8dd308e42 [FAB-17235] Fixed broken links in Chaincode for Operators release-1.4
* 835cae3d8acea9cf60074d786254d497b9c39940 [FAB-15900] Add pkcs11 section to orderer.yaml
* 3bae50c872e9f6a4539cf5524039511fb68b289a [FAB-17289] Fix gossip goroutine leak when reading msg (#439)
* 24d418d28eb31789e89707fc61c2d321ee67e0f1 [FAB-17128] Add single quote to channel name env var (#437)
* f627b8860c20039cd7c6eab3a96645ee7a18f17d Wrong protobuf import in etcdarft
* 778f87baf1415754585fe0b6ec66276af88b5cca FAB-17177] Config block shouldn't verify itself in block replication
* 0ce66851bd36a7b16fe8cf2f05a78c4b810345f6 [FAB-17220] Dynamically build TLS config in Raft client handshake
* eea42cbde1d2da59bfa87b7598627022d036fa37 Increase open file limit to address Gossip flakes
* 3a9b5e392cb1604b2f07335f6b12d9e86cc9716c Fix flaky etcdraft test by installing chaincode serially
* b4b0191c750ac988a3b03a754db59c14b9141aae Deliver can send multiple blocks when seeking newest
* 634e14bfe2b71002c44945ae66b4207d7f5c3f3d Attempt to fix flaky integration ApproveForMyOrg
* 1fe6954030ef8cee32f16cd7919d99bdbb1bc0cb Add hostconfig to build container
* 20ea5df9b871b7ca3ebeeb64c8a4ff4adaddd812 [FAB-17128] Make channel name env var
* d8fac8a92f0ef0ea8868517b9f4fcfb432e66f80 [FAB-17166] Gate UT, IT and DocBuild
* d5f056f4600226a8219cf32c3877e3b7bf84e6f6 [FAB-17132] Add Parallel Strategy to Integration Tests
* 36bf3eeeff3d88c508569fa458b0fc26edace02d [FAB-17133] Add Action to Trigger CI
* ef9960a2e9153a7b45577f1406123fc46b42c8db Add CODEOWNERS file
* d3adcc0e4c06c458bc36db3c4e8cb335e1b01e9e Fix the style-guides directory naming scheme (#309)
* c4f834d1315133e15659d54bbd1a376b69d49e39 [FAB-17115] Update doc for GitHub migration
* 2c3282e99bb9e9bf6b65be596c32353feae5c9dc [FAB-17114] Add AZP support for Fabric
* 99989784afb419fd6c0fc2d935de7f184ee99dea [FAB-16712] Update Java chaincode doc links
* 633cfbf007d0393b673fad6f8b4823a9d5f7413b [FAB-17072] Prepare for next fabric rel v1.4.5
* a192322f7d3086fde655b6e2b1fd15c68e8db49a Merge "Release fabric v1.4.4" into release-1.4
* 456ca1d9d903543215d966ca86129b7dd76ceaf7 Merge "Add consensus type ectdraft in orderer/README.md" into release-1.4
* cb15403f97cbc03d2d6b1fb85c644da480b7c9a5 Merge "[FAB-17032] Fix some errors in the doc." into release-1.4
* 7917a40ff6f694b34c971b1f8285de8b1ac39777 Release fabric v1.4.4
* a3a9485015dc5f75c31535032cfb379af0d2732f [FAB-17068] Add doc for /version endpoint
* 95ffcdc7235e46d72430ba256b7a9c9ae530a2c2 [FAB-15814] Add endpoint for versioning metadata
* e3691691d4389a93fea4c1fb20f062409cfb0c20 Merge "Do not require reboot when re-adding consenter" into release-1.4
* 06f4ad838d7344dbedc6d309786ec79cc8bf6377 [FAB-17060] Remove s390x from multiarch script
* 9f8168f3353cc2864b01ef2f218ec045e087a550 [FAB-17032] Fix some errors in the doc.
* 707f763648146fbbc4eb5171c1fbaf4720492661 FAB-16544 Homogenize orderer endpoint overrides
* 07db0a8f8748df4dbd151e357db709b5919f88f3 Do not require reboot when re-adding consenter
* 89655c396a8c0c32c9d72f943eb2ba76c0c9d099 Add consensus type ectdraft in orderer/README.md
* 3257ed616baf9d0b745ad91e3b747327208465fb Merge "FAB-16544 IT for orderer endpoint overrides" into release-1.4
* 4ca163c3c2fd8859012b76d882baa8143647b02b Merge changes Ide0d1e75,I83a9f78b into release-1.4
* 9893adf7a79a5ae96b1b4b4ffe8613ba8f21563c Merge "[FAB-15389] Fix private data dissemination" into release-1.4
* 057193472b7d1687720a013d024879e4aadb44b9 Merge "Complete chaincode execution on stream termination" into release-1.4
* 96028fd178d3e10202f68d66fff8407ad314e4b2 [FAB-15389] Fix private data dissemination
* 872fffe8d4ec268f3a2ae64d6194e817e2dd00f0 Merge "[FAB-17000] Warn when cert expiration is nigh" into release-1.4
* 1989eeecf9fa92436f735230e4fcf344b116c87e [FAB-17000] Warn when cert expiration is nigh
* c77496c658ffad40adfb8fd0d1229cbf61df8d79 Complete chaincode execution on stream termination
* 5416aeff804939b5681b81811a6771cdf31fdc9d FAB-16544 IT for orderer endpoint overrides
* 66f3d963ded5285f9167dd6f3efe577c88625dd4 Merge "FAB-16852 Update doc to Go v1.12.12" into release-1.4
* e7ed5e85848b9b6b88070a6930ea34829e7d714b Merge "FAB-16852 Update Go to v1.12.12" into release-1.4
* 83e3cb44ee7b55b2a31613ab68e77efec243d418 FAB-16852 Update doc to Go v1.12.12
* 68093d0395a798830ac397685fc466af5708f0c1 Merge "Clarify configtx.yaml capability settings" into release-1.4
* 4b0e9956db6ce64e2d1ab91a7e67b08d7eecfc1d Add Info message for delivery client
* d7f89627f71ccf47f43c6c6e36b6132f8b5c7d8d FAB-16852 Update Go to v1.12.12
* 1a1c71a9004b9f44c15fd2a918849f57abe2fe34 FAB-16544 Backport orderer TLS cert overrides
* 63e1563f6274bc2dc6d0de7f54f677eb473fd83b FAB-16544 Fix IT UpdateChannel to match doc
* 1ac3f05847279f87da5daf81415a02b89048c2e9 Merge "FAB-16980 add lock to UpdateEndpoints" into release-1.4
* 5879cd3b459ba2ac7478335ccece43fc2890d6d9 FAB-16980 add lock to UpdateEndpoints
* 31f85f6ed0ef2cc491f1041104b7ec3558f8fc5e [FAB-14819] Remove duplicate call to GetTxReadWriteSet
* 3b7b8f0f1fe246d70a9f5350363353566399a10c [FAB-16948] To make same with github
* 8196d66cb609a29c87ccba62e5c051c6d3dc8319 [FAB-16948] Fabric go cid interface enhancement
* 0c221f49da2667c9298ce36fdcd1a606f35927cf [FAB-16932] Typo in Chaincode Command
* 1485c3dce18306c30d3131af7a44e4005d4b5461 Clarify configtx.yaml capability settings
* dc14773b858928bdfd6f3d0281f4247dbe2398cb [FAB-16922] Symbol encoding format error in doc
* d0eecbac79d5789c0a8a82c95a646657418a3461 [FAB-16885] Doc usage of salt for private data
* 3d49575d2abf3afee6378adfaabf16544c80ae71 Fix Raft UT flake by prolong eventual timeout
* f71cfc74cc7f13a6bd8920752b8ebfe32fa64cdf Merge "[FAB-16873] fix cryptogen server TLS to admins" into release-1.4
* 76383ac88f7689af15444afd7578a1564cea6afd FAB-16883 fix kafka.rst doc formatting
* d6669bf855b80f039f11af3c41e820f483dd4ee5 [FAB-16873] fix cryptogen server TLS to admins
* a2bdb348b07b1a1f5c3a2c1158a2db91af7a90ef FAB-16868: fix `txn` typo error in documents
* 76efd6d96ede33c31c860905e6856a504093abcd [FAB-16881] sample configtx.yaml comment fix
* 5cbfc4f561564e4399daa39af8724340a2ea6868 Set DOCKER_DYNAMIC_LINK to true
* 59d4adce36d2ed1a8c22b1ea0de9f77879a9f53e [FAB-16756] kafka migration guide fix
* 93d94f8b6434dd54e7b70738ff7137d046a9ca96 Merge "[FAB-16241] update documentation" into release-1.4
* cea596aad0b619398353b28551e2db4a4f43392a [FAB-16783] the cryptogen gen admin cert ou error
* 81953e5fd568d524c2045460075162e8b28c6091 [FAB-16652] check for empty acl api ref
* b0de1515b910584d09aed850fc0da2d089b256b4 [FAB-16241] update documentation
* 0c9848a42411df1acfbcd146cf059827ddfe39c4 [FAB-16052] Fix peerchaincode doc
* 035b95aaa0aed6ef32d48c4315525b36bbef69b2 Merge "FAB-16643 - Fix a bug in pvt data reconciliation" into release-1.4
* 0acd6e9fb45b98fa06f0b2554b3df0f3fb3f83b6 FAB-16643 - Fix a bug in pvt data reconciliation
* 6197789fac29cd64884497c2693268b450dc2092 [FAB-16651] Fix conn leak if certs renewed
* 54f027d7e94c08255144f113d4423a2ff869a8a5 Fabric update to baseimage 0.4.16
* 36249d7c0ada3f24bf9735d87906ec96e635a943 Merge "[FAB-16729] Remove extra "now" typo" into release-1.4
* 456e9ad0195c496ac29f50c1e91c4e512476dbb9 FAB-16715 Wire orderer endpoint overrides via config
* 0953c6975eefd112702cd6f6f53b8e1ed753516c Merge "FAB-16695 Enable split admin, cluster ports in IT" into release-1.4
* 3345371f46ee7c1d204435cc838646071c80f6d1 FAB-16695 Enable split admin, cluster ports in IT
* d764996c9824c29c143f75fe7267c36e1cc05340 Merge "FAB-16715 Wire endpoint override in UpdateEndpoints" into release-1.4
* be3de21ff6813564ea49b876ed4c99ef79080e6a Merge "FAB-16715 Add overrides to ConnectionCriteria" into release-1.4
* 04d7258cf58f79a9e74431aa7f041f348163af24 Merge "[FAB-16728] Remove extra unneeded "be"" into release-1.4
* d28741a04dc8c5b3bd746839403f92f53231af7c Merge "FAB-16687 reduce mutex contention in validator" into release-1.4
* 0554664999642ba9ef17cc40a490d7f4ef23e097 [FAB-16729] Remove extra "now" typo
* a78be9146a99fe6aa4120f4c31e0d0a701b6d4d2 [IN-68] Add default GitHub SECURITY policy
* bbb36166413e0dd510d66a8e44f95e4cef0d7e56 [FAB-16728] Remove extra unneeded "be"
* 23de84456270c850afeb0d00ac438ae7577494e0 FAB-16695 Make peerServer singleton a slice
* ad1b514d976152736d27503606fb870ba93f4553 FAB-16695 Re-use metrics for comm GRPCServer
* 1a4ff3f9c16b1b6e9dd478f8268119b20938453f FAB-16715 Wire endpoint override in UpdateEndpoints
* 994f15c0e94422b3c244841346027d6f2c6888db FAB-16715 Add overrides to ConnectionCriteria
* 0ac4069228aff1558e4dcbe5606b593a332048e0 [FAB-16706] remove validate ledger
* b6fdef9ebd9a86a328d1aa113434671d3e1fc0da Merge "FAB-16483 Improve error message" into release-1.4
* cdaa9ddf2860e011fa5f4f607eee104d02175921 FAB-16483 Improve error message
* 19c28298bc8add002aa96fabe082e1ce4c415681 Merge "[FAB-16274] - Add link to off_chain_data sample" into release-1.4
* 14e85cedd21c6e2f487e70b424313447fe04f50d [FAB-16274] - Add link to off_chain_data sample
* 7775c13190847225c9f6b574a239dc3e5092bea8 FAB-15666 Pass NetworkMode in DockerBuildOptions
* 003c8c5ecc6bf11572bb00370ad842a790be6cd6 Add test for deployImage
* 1483166be80ee8733d73d229abb5d081b563a0e2 FAB-16687 reduce mutex contention in validator
* bc2d289d67002f2bcccc84a277e92c693afe6a72 [FAB-16630] Fix comment error
* fcfd12e5f361f75e9c13761df67c32cfd08c49d4 [FAB-16165] Change pkcs11 test keystore directory
* e09c726ea1484664efa7fb19a8dfcc0519ab713b Merge "FAB-16605 Add log message for slow WAL" into release-1.4
* 0abcce8f4a1d914f162a8450ac44b7b9b7a34eb3 FAB-16650 align sentence for eventclient readme
* a5d9a93feb5410931e61ce85478fe0c962d3dfaf FAB-16605 Add log message for slow WAL
* 6cfdc7d87c4fcb522e4bad249723a89ff2494408 Merge "[FAB-16571] Fix peer panic when package java chaincode" into release-1.4
* 157f500e5520e7f14d5fac09ac709e749ba4536e [FAB-16571] Fix peer panic when package java chaincode
* 7f1abdb0742ab3f613c4fe3b9bba4d5b7ab2a525 [FAB-16580] Remove Hyperledger Composer references
* 86fcc446631a9c00911e34a1324f7e39f83086d1 Merge "[FAB-16376] MSP_1.4.3: support for admincerts" into release-1.4

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=33610&view=logs).</details>
            </td>
        </tr>
    </table>
[View on GitHub](https://github.com/hyperledger/fabric/releases/tag/v1.4.12){: .btn }
    <span class="right-align">
        Created At 2021-04-23 19:56:25 +0000 UTC
    </span>
</div>

