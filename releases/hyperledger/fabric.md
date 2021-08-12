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
                    v2.4.0-beta
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.4.0-beta
                </span>
            </td>
            <td>
                v2.4.0-beta Release Notes - August 12, 2021
===========================================

New features
------------

**[FABGW-1] Fabric Gateway**

The Hyperledger Fabric v2.4.0 Beta contains the new Fabric Gateway feature.

The Fabric Gateway is a new component that will implement much of the high-level 'gateway' programming model in the Fabric peer,
enabling the removal of much of the transaction submission and query logic from client applications, and shifting it to a common gateway component running within the Fabric peer.
The various client SDKs can therefore be slimmer, more consistent, and require less maintenance.

The Fabric Gateway will also simplify the administrative overhead of running a Fabric network because client applications
will be able to connect and submit transactions via a single network port rather than the current situation where ports
have to be opened from a client application to multiple peers across potentially multiple organizations.

The Fabric Gateway is delivered along with slim SDKs in the [https://github.com/hyperledger/fabric-gateway](https://github.com/hyperledger/fabric-gateway) repository.
Check out the [client application samples](https://github.com/hyperledger/fabric-gateway/tree/main/samples).

**[FAB-11334] Unjoin a channel from a peer**

The new command `peer node unjoin` enables an administrator to remove (unjoin) a channel from a peer.
The peer must be stopped when the command is executed so that channel artifacts can be cleaned up.
The channel's blockchain, state database, and associated entries will be removed from the peer.
When the peer is restarted it will no longer receive blocks for the channel.

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

**peer and orderer - Default log record format improvements**

Expanded the width of the log record sequence number to a minimum of four characters,
moved the log sequence number and log level to the left,
and added bold formatting to the function name.
These changes keep the fixed-width columns together at the left
and add a visual break between the logging module name and log message text.

**peer - New configuration option to disable gossip block forwarding**

If all peers in an organization explicitly set "peer.deliveryclient.blockGossipEnabled" to false,
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

**peer - Ability to override core.yaml chaincode.externalBuilders via environment variable**

Since chaincode.externalBuilders is an array, it previously was not possible to set via environment variable override.
It is now possible to override chaincode.externalBuilders using an environment variable
using the format `CORE_CHAINCODE_EXTERNALBUILDERS=[{name: x, path: dir1}, {name: y, path: dir2}]`.


Fixes
-----
All fixes as of v2.3.2 are included in v2.4.0-beta. Additionally, the following fixes are made in v2.4.0-beta.

**orderer - [FAB-18521] Consenters' metadata is not replicated while OSN catches up with snapshot**

If an ordering service node crashes while replicating blocks from another ordering service,
the consenters metadata will not be available and the ordering service node will not be
able to reconnect to the consenter set upon restart. This fix ensures that an ordering
service node that is replicating blocks persists the consenters metadata so that it
can reconnect to the consenter set.


Dependencies
------------
Fabric v2.4.0-alpha has been tested with the following dependencies:
* Go 1.15.7
* CouchDB v3.1.1
* Alpine images 3.13

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

* a330b66e8c9f2d71d1d00812d481fd710de3942a Add release notes for v2.4.0-beta release
* dac896a3cb13067ea9811fb21d87a0d74e78898b Add slash command for invalid issue
* 474baddc1c381c347b5bc02cf54e5a1113b5a88b Better error messages from Gateway
* 497a177ffb818ed8f75578cb55a65ba2224a85ea Fix FAB-18528: remove panic in ifConfig func (#2828)
* c41ffff8d20831d26acdf84899252c49a894e733 Fix small doc errors (#2816)
* 99d2e32a5b994479538b768a11a525546b556e03 Output File Exists Error
* ea48474507ed0d7e7f30af33bc58c1c319b8fa37 [FAB-11334] Adds a 'peer node unjoin' CLI entrypoint to unjoin a peer from a channel (#2769)
* 87ea070abead1c9df5b42d54a2ff8fae21ba5c63 Gateway enabled by default
* 5331bbce68c3fa79e98bc08a6c997093ff7cbd13 FAB-18067 Discovery support Implicit Collections (#2784)
* 240cf0e182938a09832ba4162c3c229c81848e3f Merge and enhance coding guidelines across github and wiki
<details><summary><b>See More</b></summary>

* bb8bada7b864d4135aafe1785674be31d6cc78cb [FAB-11334] Adds a function to purge a ledger's transient storage (#2769)
* f662d9829176ac7bfb5129d45b486436790b404b FABGW-25 Endorse using generated ChaincodeInterest (#2773)
* 71037f3b500da9bac9557d1cd5d292e16eee1205 Update CHANGELOG.md
* 95fb683a4073163f7c16d62e6959fd1d4b7ea2a2 Hardening raft catchup IT
* 463271e0031c583510cf59a2b1ee777f19803083 FAB 18365 evictionsuspicion failing when osn failed (#2780)
* fe7147445ae30ca9732a71effa4f05937ee48ba3 Additional documentation for implicit private data collections
* fa3960b33e83bc82117ba742f4710f8390219fd9 FABGW-25 Test for system chaincode (#2771) [ #2767 ]
* 52b12dc47dac69a6bab6b7fe68f304176b57304d Update private data docs - remove SDK reference (#2770)
* 26ec54a6c8236a2ba71146b7e57a18c66d46bd05 FABGW-25 Build ChaincodeInterest in TX simulator (#2767)
* e5e623d92b74772f30246ecd0ebfd0274ae4bae2 [FAB-18527] Discovery supports DisregardNamespacePolicy hint from client (#2768)
* 9a922fd9c78c01d185bc2b45fb98012a37f7bfb9 [FAB-18527] Discovery supports state based endorsement queries (#2764)
* 84c1270776d1c8612f4cd97cc837e4fbee4930d6 [FABGW-25] Move chaincode interest to proposal response proto (#2763)
* ffe7d363ca22adba185833b4d9014592bc1c62f9 [FAB-18521] Fixing flaky IT, send remove tx to another node (#2761) [ #2748 ]
* 44ab2bf96cf0d304a2f1d8f8b8cdd843e2279381 [FAB-18521] Replicate block metadata with block while OSN catching up (#2748)
* 2c6986347ede8163793fb9971fb1d1211f31ace2 Update test network tutorial for new profile
* e4b66f98447539566979db67f2dd6f1f31b9da77 Update boostrap.sh for test network
* cf263b08bb2de22f71ebda609b7ef89d4476519f [FAB-11334] Scrubs partially constructed/deleted ledgers at peer init (#2754)
* 62cd59ca2ee7e37f82ed7e9bc7b08cb9f6822df0 fixed peer documents
* f7f77af161b9574b920e49288c7f1873e57c7986 fixed peer sample config
* fda47c5437d35b18c60ac3155d4548287853f695 Renamed Ledger Binary To Ledgerutil (#2746)
* 973648572eed0cec2bf0002252e31a95658d865c [FAB-11334] Adds a new 'peer node unjoin' feature (#2732)
* 73c46a1c07c551a492c9e8e8205998fbe45f7caa Updated enrollUser function in write_first_app Doc (#2713)
* 965664fcf97a2b429a5230f9209e3181bedb69f9 Update docs to clarify that an implicit collection can not have an index
* 1249da2598549b3a7b03bceb0c29c19664c24c25 [FAB-18509] Stop panic of collection index path is wrong (#2726)
* 9c3d4591a5c3ef30f76fdd3b9da926861aa5f7e4 [FAB-18508] ledger utility always outputs txNum (#2724)
* 4c4e58c1228968cefc9d5c027f10884fb3707174 File Location Flag (#2709)
* b5e0d27b855242d51d4fdc7c422a3f7297c51b60 Added a possibility to override chaincode.externalBuilders via env variable (#2643)
* 1f1c303eb8458f047047f96beb4acad344d0b50e fix typo
* b03422528ba9fbbe824f2c4f9242f9174385f5c7 [Doc-Update] + What is a commercial paper section
* 1ee03b33d1cf6beb509aa0e9ad45139b05ccd922 Add function to delete the ledger data for a channel (#2722)
* 7151302be2dff77a9d78cdc8c7a04c4fee352914 Fixed grammatical errors
* 4e2f86e71c2fd06d1aa86a41fb0fb6729f455504 Fix a typo in CouchDB tutorial
* 3a75b656f27f6bbb3e0518dbc93b86f5d6212d2d Use protoc-gen-go 1.3.3 for generating protos [ #2113 ]
* 8ce450eb339eb5005f7dbe99100ae6d023a2761f Fix typo
* 4422a1990b9a12f1bfd4ff98910f4ed2d16946e5 Fix peerchaincode.md as well
* 4e67cbee43cc60000af51aaaec5c25d935f5b19d Add explanation of `--ctor` JSON string
* cdd5a046953b0d1ed55fc3bd1e43cf30b8d777cc Compare Snapshots Utility
* d80cd2a6955e86f393b08d2335bc92a5194f30ba Clarify Verify behaviour in PKCS11 Impl
* d55dc8e13609575316f2c65604e904f4cd7c8776 fix typo (#2695)
* 8689771138c15bdb6171844768e87ad3531975c5 Retire Will Lahti as maintainer (#2704)
* 16259ed70a4cd57513be40a0678213d9274a9ae8 Mandate TLS 1.2 or higher in fabhttp package
* b5a4fe942ea819011e403aeb843ad6f62564ffd4 Address PR comments in Gateway integration tests
* 52c09b61f0cc7df4437652f22ec56a75e45a7e87 Clarify orderers seeing the transaction data
* aa0b33fdf7692f40e567d6a0b82840f4ec1593b4 Retire Brett Logan as maintainer
* 00910bad821d98b0111e81bc5fc02677618fac5f Handle missing endpoints from discovery
* dc09b6e7d0fe359ae21d3d52e1e16f37f593a3a6 Cherry pick deploy CC fixes to main branch
* fd218eb650c9c97ba6f4a9ca9c4c21f8ad857fb6 Clarify "identity expired" error messages (#2685)
* d9e850d3b840ada6d493fece92e90933f69770cb Fix spelling mistakes in the Github Contributions page
* 3c7fa86dcaa085e5d13661f5e129d11abc2c63b8 [FAB-18484] Return transaction forwarding result back to the client synchronously
* 6fbca4945531679f903d71e10af20a5a01c5537f Update Artem Barger email address (#2671)
* c81f265d79c797a133f92c346b813ee7a0710134 Link fixes detailed in FAB-18494
* 266497f99abeb5482947cb7e674f566349ffec0d Typo fix in peer deployment guide in main (#2660)
* b4cd030bb5c8ed79529cff05ef1653ede90d0c70 Link fixes in create channel tutorial (#2661)
* dde41d9f1e8c2ef2941f1b88b2afaa789fc920a9 Fix link in orderer deployment guide in main
* b2f7292925d2dc28f296e5772b2c903c0a4d4d25 Improve mvcc log warnings (#2649)
* 04796e6f00aab5b4ff53dfe31469a682cf472ea3 Use protobuf Getters to avoid nil reference (#2646)
* 07808a0feb5e37bb139fc5ce3f75364842d2fbfb Clarify doc for readset validations (#2647)
* a8dbb689ea64c9d679eee79f622d55fe1f0e706b FABGW-20 Implement TargetOrgs for Evaluate() (#2642)
* 85ae90c1bf097f8890bdbbb51d60a768126b4a2a Added RetrieveBlockByNumber into blockledger (#2635)
* 1ad442277eb371e32f07f583762b84af5496290f Update secured_private_asset_transfer_tutorial.md
* 1f89be968af014c85011fe1e76a7988466071691 FABGW-21: Realtime implementation of ChaincodeEvents service (#2604)
* 34a41866abb92fd92cdf49703eba89a37da349f1 Fix minor code comment
* 9170feac42236f7f6d796d8ee05e703564acf9e8 Return block number along with validation code (#2614)
* e8e39e6dfcceb14a4998d6ea64542d9d8a7b825b [FAB-18479] Log error if orderer can't forward SubmitRequest to Raft leader
* f1fc4996861f35a1b7051ff2ba7b0ac385afdf76 fix duplicate entry in code snippet
* 17dc11c90cce7df2b71d8a42e094df5aeb0c1a14 Update Building docs to reflect UI changes
* 0334d52827d11bdb3b6352cc8cc0cf624f81e753 replace brew cask install --appdir='/Applications' docker with brew install --cask docker
* 4e201afc69efb6d6546e1be904c5e658ca56b9a0 Optionally disable gossip block forwarding (#2606)
* b4efe857ffad1e84877650f192e6ac27d143716f FABGW-20 Specify endorsing organizations (#2578)
* 6f0bef10331a976d1daf7a40922c1faafae5c6fb Bump vmImage to Ubuntu-20.04
* f8070ecb27250a70328c4255f0de8e2f4905aab9 Maintain order of transactions in the commit notification
* cca66b67fa32b6b9c7f9f33496f53af2a92707d8 Add chaincode events in the commit notification
* 885e83dc83fdc5d9a5f3ad92866c65cf3379e12b FABGW-18: Fix concurrency issue in commit notifier close (#2599)
* 856c5a1c7551db71fe86b0c0228381e291d215b1 Update docs/source/upgrade_to_newest_version.md
* d296963ca9903433c9103489e175a40e52d93dbd Govendor added to documentation
* 13bcf3f7d910726e2cfb5b5895f9aa51d232b1a7 Improve Logging When Data File Does Not Exist (#2586)
* dbf7eb127365cb1fcc517360b3bde9bae79bf2bb Improve error message for invalid consenter cert (#2587)
* 5e1e590fc041461ebe40de1a90129fb2e138247a fix typo
* b20d356adfe2e7b3ef304ac04e07e5108776d84d fix typo
* 318510f80ac41ffe9df3b628c495ad8bb738f0f8 modify some errors
* c73f893a1657f51b0206423b6fd685fe9b1fe230 Revert "Simplify GitHub Action for AZP Triggering"
* 1866adebb2e69a74b70bfb202eda900740f9c6aa FABGW-19: Secure CommitStatus service (#2570)
* df8c049f248b29331c444c91f03877bb6d7b1963 fix typo
* c03ccf8c487a7e8f8af1f8f2d8ca058a101cd858 Fix incorrect error message in Gateway submit
* edd0f040ba354e2755764e3703aef5729556d49e fix typo (#2569)
* 2d504026e664c689d65ef7b479a040bb94892ebd Add log warning for unathorized operations requests (#2567)
* 627f9639deff8982ad6e91d100d23aec43d827cf Corrected function name in comments (#2568)
* ef59964c19ce6abc11a9d61699a24e822778abb1 Removed early mentioning of organization R3
* f2c0f8e161c6ceae6ccecec5f4bb36ef8120e70b Updates in main branch for release v2.3.2
* 379862419dab233657b41d90fd1819ba498737cb fix typo (#2564)
* b96fa099ceb461d78a416695d5e7e340529584bf Add debug for policy defaults (#2559)
* 12f9b4081d38ddb29ffd451514bd480e684a6c50 Remove redundant casts (#2558)
* bd640c8acbd77891e22931ad374e9c9e7988a52f Remove redundant comma (#2557)
* 7db78b3ebb0ec440ba49982b00fc03f51819b410 Remove redundant type cast
* ed1026c53d0601dbb0f095c760e0022b97b302d4 fix typo
* 6790f428b3c4c57f8000a7653077571b88244fa3 fix typo
* d5ab07292526376b6d364878f618015287e0a219 fix typo
* 7c9122489366eb66983229bec850c05d3d0b011b Prepare for next release v2.4.0
* deecdf980458165756a39eba0f30bc1b8a08e44e Update email addresses (#2544)
* a18f1c7b9ad6e0c6614de26f277d38183dab5270 Fix Typo
* 92ca023865c857dbb83bfbe9339b7b392c963b8a Fixed grammar in docs for membership
* 06509ad2fda9cce6098d900bee99dfb8eeb7a628 v2.4.0-alpha release notes
* 4365412733e4be7496b24c1c7bc5540aef0e6993 remove redundant slice cast
* 5d500ee83c71216acacc81b9606a50cddd05accb Fixed Typo
* d001dbc9961045bcb680978fbdb6a59e2ef9901f Add debug for gateway endorsement requests (#2538)
* 4cfc722d0ffef35a4ac8b0ebe17eea4dcc3b1018 Skip plugin tests when the noplugin tag is used (#2535)
* ba7e92358b182995fb1cbea3b0c5c31361321d72 fix: fix typo
* dead74ff9d009105344b07b0f26a657eada61563 Fixed Typo (#2533)
* c7dc5d7ae4bd1be4657c03bb0d708013c34f675d Improve snapshot dir error message
* 3714ca3cbaa003e9785f1aa4468cdcfc03bd76c5 Document ledger.snapshots.rootDir
* b1f43299ac7a3325bd686e1d34869b170b1fcc51 Simplify GitHub Action for AZP Triggering
* a8bfc985abc1c86b7f800d6a28518e24e25e9faa Update deploy_chaincode.md
* 345a08b5cd30ef937a8270d1722462e4cad1caa9 Add Security Model topic to docs
* aefa755a9eee3818fed5cd5f9070b922f0aa1280 Fix link in `international_languages.md`
* a559b2cddc6aa04bec56c59520ae54041dc01ff0 Fix timeout in orderer connection from gateway
* d88e09c9a36b1e5f795820003c49555f0da325c8 peer: the 'noplugin' build tag disables plugins
* f5de4312a81a0440ce5819dd8e160eb68aec83b7 FABGW-9 Select endorsers with max block height
* f4dba9dca8906d12d08eba01dd92bfe18dfc715f Fix old or incorrect contents in the doc build instruction
* 576d186581cc8acb39e21ffbc56d96de9f7ec9eb Fix the fix for race condition in Finder unit test (#2504)
* 1147977a810ac58c97bd9429b052cc9b56e496b0 Clarify private data doc for endorsement policies (#2502)
* 1cc0ed0e7be50dc668408d38b48ec76242a78acf Clarify private data doc related to private data responses. (#2501)
* 7ac0b60cc0e66ca49016be6434a879c6aea41a19 FABGW-8: Fix race condition in Finder unit test
* 62e327e9b5b71403220a667dd3ad01c46bce957a FABGW-8: Implement Gateway CommitStatus service
* a1d06ebfc721ab9d3661e49ea84e765c9825101f Wire function parameter to its actual usage (#2499)
* 4793d86fafd10de296b56cdfbca835bf951d0acb build(deps): bump jinja2 from 2.10.1 to 2.11.3 in /docs
* 54e27a66812845985c5c067d7f5244a05c6e719b Update "master" branch references to "main".
* c0ca3c29b18404d21409562bb5e4a5dba7685577 Regression test for prev commit "Bugfix: loadLastConfig wrongly returns nil instead of error"
* a54199b1416edff47377ae63419a6693018ae347 FABGW-8: Hook commit notifier into Gateway service
* 13092bbfb631a612091d4ccd3e849b320fa9c6a6 Bugfix: loadLastConfig wrongly returns nil instead of error
* 18b78dab9aa148e1a833a9637fbd964738b3dfc3 integration: PKCS#11 SKI to CKA_ID mapping test
* 5484a18d3d713f541dd9e8551cffe35bf52692ec pkcs11: Add SKI to CKA_ID mapping for BCCSP [ #11 ]
* 178de674201abf9e6c3b15dbbdf3925e7222b56b nwo: capture config file updates through network
* fffb2bfdcaeccd99958fc17ec13132dcf3b7a6df docs: Add some comments about untested code
* fd72843ae1ac896d671686af5b6283ad3002f2f9 Handle unsuccessful status from Gateway orderer send
* 9319f4a0f0d8fffbc17d0407db5578725a61c112 Prepared tx must be signed before submission
* ab79e69fb5ba076f3220d60ee03e3615846a3edb FABGW-8: Tidy up commit notifier
* fad002c11ee3b6f106c4a2c47652cbad1dac1e59 Gateway error logic refactor
* 5ff76d38c7902bc0c8dae2ce38cb02bde75a4953 Tidy up gateway unit tests
* 76763d1b8900df79080765453f944122dd7d68aa FABGW-8: Wait for transaction commits
* b40f703dd168c5f98e2e17a8fe719e89ea35925f platform/golang: loosen assertion for Go 1.16.2 (#2480)
* fd62c39ebc8663d5a8527c1a1e804eb539772c7c msp/mgmt: remove reflect based type assertion
* e5827c522e676ae7917d0d66b66b33392f070831 lscc: remove GetManagerForChain from prod code
* 2c7c37ddfe3ed2ac3417348fcd75831b17c79f36 peer: remove GetManagerFromChain from prod code
* ba6a87eca4110786c4c1e7f0f537e2a3b4632d24 peer: use MSPManager from bundle instead of mspmgmt
* 86d1d0abc8870cfeb760da9f0d59d6aa4e3fe8e9 common: remove the unused common/config package
* 85dbd43aeb2cc105d04f2b4851a11ee4592a749b cscc: stop wiring policy.PolicyChecker
* 7204344c64313bda5ab2188c2cef007a9ecf75c5 peer: remove NewConfigSupport and friends
* e2218d72d094b5f37cd9d16545f70ad81150ff9e msp/mgmt: remove Setup/Deserialize wrappers
* c40cce0abe30c2e335d09ca060d55a2b6393a73a msp/mgmt: remove LoadLocalMsp
* 50406fea6f1e52754433a22a25b8efab5e1bfee9 msp/mgmt: remove LoadLocalMspWithType
* 8e3751ae0e429d26388d28665e256925c5279070 msp/mgmt: remove GetLocalSigningIdentityOrPanic
* c4eb80f8953a29b6b2bb010517da664be290f8f0 peer: stop using GetLocalSigningIdentityOrPanic
* 10b09b9c8fc71dbc83c17dbf45dddae593fb15dd msp/mgmt: move TestLocalMSP into mgmt_test
* 1dbd6e9bd93ec897ec84720490a654e110a1f13f msp/mgmt: move MSPPrincipalGetter to policy
* bfa7dcf5ab835e8e122ad504b0397efe1a3aa895 Remove unused policy checker from lscc
* e6a04b90187cb1506c795124135eff6a9c83accf msp/mgmt: move DeserializersManager its user
* ed964d3704481a7be88a215de8e0962139e94f33 msp: construct DeserializersManager  with local MSP
* 0c28b4ee32039d2dbbe1b1a6be018f0d58308c34 Update Gateway with latest fabric-proto-go version
* dc5cecae8bd7221c2a3fe85c1c329d64f361993c Implementation for commit notification events for embedded gateway.
* 73d6539bdbf8c19b0cda143638fdb6bc0af3e879 Gateway gRPC functions to return google.rpc.Status
* 8edf5137ff79b59a64f6dbc9be375e2e5bf7ef94 Update fabric-proto-go to latest version
* 2d81cb2fa65dafb5385dee262775df6b930dc49c FABGW-6 endpoint factory to use refactored comms
* e71b99ac6895519354b7364a1642e5aeadf6946e Provide commit events from ledger (#2470)
* 69b636c4816ea349e555ee6b8384716d1cf0ed6e Run `go mod tidy` with the latest Go version
* 82096464db8033f39191729acd7864870a586dd9 Remove un-needed casts in discovery_impl.go (#2469)
* 0afd4042c6a28c9fee3ad6c688a9a9a58fffa131 Upgrade goleveldb
* 542f3207d65378cf95cdeaccbe1c0e20aa65178a comm: move GetLocalIP to its caller
* acceb088bd40048944cdb18d9e5a36237bf7e05a comm: move cert extraction to common/util
* ef156bd7fb65aa244e62f6ce7aa2410a1a3def91 comm: move BindingInspector to its consumer
* a2f2fa51e524ccececd671293b56310e449ed4f5 comm: remove AddPemToCertPool
* 61ecf96b0596acf87dbd04eb016478f894be6311 comm: remove GRPCClient structure
* 701ef1636bd44bd34a2ca25db9ab5f022b1d080a comm: get dial options from config at new conn
* 505b91780f3ff17a4ba5bfc4a3ab100446669be2 comm: remove unused fixtures from testdata
* 1767b5587aa05b6b82935f5f93b5078daf686ff5 comm: remove TLSOption list from NewConnection
* 3a91146f7e75475b12ff7d892d3a3598b735c236 deliverservice: update DialerAdapter signature
* a4027020a9f1ec4cfc395a7a40153ad78ddd09d9 deliverservice: replace CertPool PEM certs
* ac5fd790b7c5ce23393370d72398277ba6a30afb comm: stop passing GRPCConnection to deliver svc
* 933ac903e546d8c915a4e43c6a422537780ff940 comm: move ServerNameOverride to SecureOptions
* 52427426f4763d8b09d81480bf0c7b6c3cf15fbf comm: remove GRPCClient#SetServerRootCAs
* ca15dc45290029679bf941eaec55b32498b22df4 comm: remove GRPCClient#TLSEnabled
* 8c7cb70263cc1a789b36bc51032d6a9f713bfb95 comm: move Certificate to SecureOptions#ClientCert
* 8ae44de6a670867da114fcc492f3e7a1d9a00d6b comm: remove MutualTLSRequired from GRPCClient
* e7b9c3850aaf78f14ebefc0a8498e420dfb976d6 comm: ClientConfig builds the grpc.DialOption list
* d94463384b6fde05b66087243b601abb2029967e comm: rename ClientConfig#Timeout to DialTimeout
* 6281c0cda329df25c8ca86bd1e52e19f0632c1c6 comm: SecureOptions used to build TLSConfig
* e0fbdf3b34510ff6b4bf4b029fddff3e3c4d8ac3 comm: hang option accessors off KeepaliveOptions
* ab9ff142301057130d9f7a46fe4227592664376b comm: remove ClientConfig#Clone
* 4829636c4709194cb4d707df213afb6a7e7988c4 Add a note explaining channel name restrictions on test network tutorial
* 9ac47b13e26595af4be0fe3c78cc4fd79e1fd012 FABGW-6 Use concurrent go routines for endorsement
* 6279191a02eb88000882b1e19f81aea9c8f40f69 Initial gateway integration tests
* 4a37575d4d7e8ec5b7b16332ba8565fe70ec4e72 Update Prereq, Install, and SDK docs
* 15e95d630afdcbca3effc37c13e16a15cd3c38ae Docs: Update Getting Started section with install commands and add links to asset transfer basic.
* e1915a3c14ade0bee71580f012d3e4e757c6e026 Change name of comm msg size default consts
* 6a458ad372cfd0a8b92b28b263271e5c046201a4 Refactor max message sizes in comm client config
* 11636f55b72f1b6e3155900978e7079cf9c24da5 Replace WaitGroups with channels and timeouts
* fda1ee742c40f2a32e9523df38a90ab3d71274cb hygiene: minor cleanup from previous commits
* b83dacf3eaccf1d44d30e4821ae4efda22274120 Replace Config interface with ConfigUpdate struct
* 7751eaef6b7c0bea5a5cece6455163bd8783a5d7 hygiene: remove camelCase import name
* 7a8e1de06a739f730df8987b025ee6d7dc254886 FABGW-6 Implement Submit()
* 7172484f259f0106994fe97522823e7f2d4d90db protoutil: add CreateTx helper
* 21a800b07fbf9f3b927d81a4c86ade30d3ffadc5 integration: exercise osnadmin in the e2e suite
* e708729651233edcb3175640349546557d5518f6 osnadmin: add --no-status flag to remove Status
* e53b900ba0cd440f8f536ff77ebe28177177075e Add check-help-docs target to basic checks
* 7dc4d033a70871aa259369e5953d93bc4e19620e integration: throttle grpc/http client creation
* 9c3a7322d8511d66b77da53cca00e2c947f3f7f7 integration/ledger: rename commitTx argument
* 2f7896756057b116a5eb0fca74d338ec696c290c Add tools target for the tools docker image
* 5bad6aec88e576a377a65192a4eaf69e8307f5f7 deps: bump fabric-config to v0.1.0
* e0253ef0466e4e16364f3d1d3cc537ad9d8b1c4f Fix images in network concept and upload new diagrams power point
* c4e6a48ac65755b0e6c4dfa970a1653c6068b1e1 Increase build timeout for integration/pluggable
* 24da29ece1c9250f0f0cae94bfef487d758327ea integration: remove use of internal/peer/chaincode
* 6108e5b124b7e7b650dab11a27ef71d41d3898f0 integration/nwo: add grpc.ClientConn accessors
* d32d1e6e6235415796b7a1a8bce0e349d03a6616 integration/lifecycle: refactor RestartNetwork
* 95cb08aa3671767d71313e34f7d362ba602156e6 Bump Alpine to 3.13
* 51cf70802ca1fac745c6680face724ef625902a4 Add Alpine Version to Tools Image
* c73a680ecac358628cb6fb10d3029800db37e404 integration: replace custom function with matcher
* 3b15d6047f6eb96f469c790740ba92ea0385c2d1 integration: move templates to nwo/template
* 6a28a3539cfab88ee5149eca62045da16f5aa7bf integration: remove yaml network definitions
* b3e6036a1eb53bc9c365d168727f0b736e8e7701 integration: remove helpers package
* b22af03ec81f392323754735a45778c433e77366 integration: move runners under nwo/runners
* 44abc6b26d964eab9adf83d17a58e4ceb96ed39c Fix bug in snapshot request submission
* f0584c610a7b4308bbb2bf1746101d6f2d08e93e Report correct reason of stream abort in orderer cluster
* db0a8647ed249a440955485119a8583adbf921fe Log stream total lifetime
* 6c3dcc4c56a2a62c43c6c8c971345735e8a07c1e integration/raft: use nwo.Signer
* 28b9f00a86f05b441c110720a3fbc639c3f0d3ef integration/kafka: use nwo.Signer
* 99e8cd5ddc986c3d556b52d12e649c8ef294d00a integration/ledger: use nwo.Signer
* 82791882f974534bc1cffd0f71e2ebf536ddc602 integration/pvtdata: use nwo.Signer
* bd2c193d05b760355aff46ce4868f34a0820a40b integration/lifecycle: use nwo.Signer
* ff7f98d64b7d96cd7c7ab9e0e99928d59cb698d9 e2e: replace common/signer with nwo.SigningIdentity
* f8328073f054473c42d14c4123296004af3353d9 nwo: add nwo.SigningIdentity and accessors
* ecaf6970efdf2e5fde72f7c8ec903d7b3827de8a Disable connection pool in operational clients
* d3d7e0553eeb37a41fc1a5f2be1f4e2742c5954d corrected organization labels
* 316cdcd5d98af026d9bd675230a1d60cb4eb2b1f corrected Org1 text in Org2 box to Org2
* ed8d55675b8501e35d20247f0d43c45f4cd25cc8 Only run Kafka suite and ccenv-1.4 test on amd64
* 54ae5c71e55047677cf7c0e9d91607753fe9db7b Remove Kafka test from integration/network
* 4090606e65bdc16003e38604224372c269b3e66e Use busybox image for cc platform pull/build test
* 7dc39a4451bc6dc71165e75ec1463c05b3b4432d add linux/runtime.GOARCH to legacy cc package deps
* 84b332d0bc0be6e8d10267ed7451e78b92e7d863 deps: bump golang/snappy for arm64 fixes
* 33886a4febc58f7d5f1278fe2246daffb31067a7 Add binutils-gold to resolve link failures
* 5caf9f2ddddcd22883a240ce05539720cde9a65f Fix a duplicate message while orderer setting up
* f9d05b38fd291636c5cb8ab4222d21195e4837ee Update x509.CertPool equality checks

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=38994&view=logs).</details>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric/releases/tag/v2.4.0-beta" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-08-12 02:18:09 +0000 UTC
    </span>
</div>

