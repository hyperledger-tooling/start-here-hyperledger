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
                    v2.4.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.4.2
                </span>
            </td>
            <td>
                v2.4.2 Release Notes - January 28, 2022
=======================================


Fixes
-----

**peer - Discovery service does not consider full set of endorsement options**

Due to a bug in the permutation logic, the discovery service may not consider the
full set of endorsement options for a given endorsement policy, potentially resulting in the following error:
"no peer combination can satisfy the endorsement policy".
The fix ensures that all endorsement options are considered for a given endorsement policy and set of peers.

**peer - Peer gateway does not close connections to orderers that are removed from channel configuration**

The peer gateway service now closes connections to ordering service nodes when they are no longer part of any channel configuration.


Dependencies
------------
Fabric v2.4.2 has been tested with the following dependencies:
* Go 1.17.5
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

* fad7f691a9675c029bb49da14ef4a61516cc5c76 Release commit for v2.4.2
* 0e9cdb2e7ac24a5841693830ca875507dcdf636b Address windows platform in documentation [ #2993 ]
* 63a77795e130e71e0b165fe0a30cb362487fb47b Bump Go to 1.17.5 (release-2.4) (#3182) [ #3114 ]
* e24c3327fc15bf993c4568909ba4b0335f9f3344 Refactor gateway Endorse() method
* e7cb726f564dfc7db7b389fdcd62945e02db80a7 Close connections to stale ordering nodes
* e1ed78f787a7285fc528aea97177bb446e6da4e8 - Fix failure to generate all possible combinations (#3132)
* af5d5df427d41dd1a8e83bdeeff79086be2b2060 v2.4.1 release commit
* ef5ac00599d82f6067e5f253db65710d150ae665 Update 'Running a Fabric Application' tutorial for Fabric Gateway
* 3580b4e845769a5218a0f1f0fed181c78b5a9769 Reduce CPU&memory cost of collecting endorsements
* fbfdc1daac851ba36a5be938921b96992afee30f Enable gateway concurrency limits
<details><summary><b>See More</b></summary>

* 1f877095649ec9968db93ae81ff83825ea07911d Remove discovery.acl principal warning [ #3006 ]
* e0bb139ccaddeaa329a6ed814fa30e7263413dd3 Adding a dedicated external builder
* 654a02b11bbd9290345da06ad33ea344d0bb379c Fix channel config callback in gateway
* abf5d3043e618bab17bfc2d5f79f59c425c4534f Final peer for gateway (#3091) (#3095)
* 2d8d7f405ca677f3da18850a0476c9c085e5b3ff Randomize endorsement layouts
* 29d1e2137b04a10f1e1c954cd2ba7fbdfd101c0b Network and Orderers for gateway
* a95a8e72847bfa650757d80b8abbd7e32cd4bebe latest PR review comments
* 41b6586b386f66201b99059ae75fd0f0201d4c92 v2.4.0 release commit (#3078)
* 4f4e0960fa05ea2e351b9b3cedc2ee6e8171c398 Update v2.4.0 release notes
* f15b4eed7d80df7e03b34ea7146663e3c982fdea Add command reference doc for ledgerutil
* 45707acc6a4c2b1fd651be3fc21f0598d3776e34 Add read version to the example in read-write set
* b0de13907e7efb43f322ddd2adf8c9d20c0a793b Add logging for identity, policy, and signature troubleshooting
* 12669787280b1e9f268cc0d79b45ae91c3a8d78b Clarify v2.x upgrade docs (#3083)
* 6a7cdd0731c0ee1c8e8bfd61c974645cb31fb710 Refine Gateway gRPC error status codes (#3075)
* 40fea67a5bc2312eb29918230ca1ae2a2ae3bc66 goimports updates to prepare for Go 1.17 (#3070)
* c14239c76c2ea46fdb1049960d1ac610a90dd3fd Add gateway ref to private data doc topic
* a6a9fdeea7ec9af6a5eca067c1f66442b2fe4419 EndorsementTimeout should apply to each endorser
* bd1aaaeaa2e8e9fd501976accb4b6a6947490747 Reference current application APIs in peer event service docs
* 91951d0d58239fa009d191b7b2b2150a85ed5405 Log the transactionID in all log messages
* 2abb074b01b38ec998aaab38b92e826baa2c5bb4 Remove redundant SDK documentation page
* a1c13d8ac4eaff48cbcfed3b5c2623ad04504f08 Updates to endorser and gateway logging
* 34dcb8d2836afaf82f94de283b2486c166a781b2 Update protobuf definitions
* 5c2e358aaaf24cbaacc4713f5779e0f0dbd9eded Enhance gateway error logic
* 5014709f03bec81f99e7723a2543d218a88a5c4f docs: fixing some typos
* dee44d9ed5d40b40e49de9656a0fe7ac47d041d5 Don't use EndorseResponse.Result field (#3051)
* c463b328b7c9c0149a91f160b6005499d454bae6 Fix CI script syntax
* 44faa13d04a2a723e14dbb89de59c3922a18cdf3 Enable unaware threshold signature endorsement
* 8a4c7f3bdb17c18fe6c56ff7e3e2fc008e223005 Update Contract and Application API docs for Fabric Gateway (#3048)
* 91d7b7c2fef4be57fbbce6f7bb193b311d7712f4 Updates to Gateway doc topic (#3047)
* 6a415eedefcf807e7679a3564f159040f34afc49 collection singular
* e3abd6691c813116fb2655db9d5ae1a3757fcd6b use member of a collection
* da935d73f799f224a5f4911f63bb6694a78c30a2 Gateway overview edited
* 9c5e1dfe8de91a0f75bba5a7a15b366539fa5558 Clarify ProcessProposal error handling (#3044)
* f089b24b1a009b0218e7df91c942dc1b992b869b Reword evaluate() error message
* 688d4d2b27c494c15d18b124f3702cbd92378999 Add extra info to error message
* 6926cc17c0ef72d979b7fdb9c39c676f0f88f587 no gateway via cli - tutorials (#3037)
* cdc342ec1028d385afc5800e67a1adc421debb9b Add gateway architecture page to docs
* 534b1c1e0808dfda8001157ca51a7849543cdf50 Use correct timeout option (#3032)
* d67d421d6128321c500c1936e6abe98ba1004696 Show what do not match (#3012)
* 5113aa910b9c8aca8a8162d56d657d7d3a7238c0 Better gRPC error on context error from CommitStatus service
* 62fb4c0cc525cf7d6457dd37d83d4bbb3ddb94ea Update transaction flow doc for peer gateway
* 40f90c1feece5e9d696cedd960f2d132d37e18bb Fix typo in comment (#3016)
* 45f4dcbf57c6f6fe312a632cdcd2cf820d13eb02 Add chaincode err message to Evaluate err message
* 42c99e0b8563e1fed961b9e571ff9f4929e5ac40 Add documents for new options of calculatepackageid
* b1c9d43911608d2d3c716f5615bf227571746188 Add `-O json` option to `calculatepackageid`
* ee18f9dc281ef3ddbe9ecbaa3d8ac7e6eb6cf734 Return package ID without any prefix by default for calculatepackageid
* 843ff14b768a83f13168d113a267284f44eea3a1 Update Sphinx to v1.8.2
* 70ace58ae902318489894a5cd7b4e6ecea00bb5e Add integration tests for `calculatepackageid` command
* abdb330c61d37f8be7f02ceb1d85378678dee557 Add explanation of stringArray
* 89da86e59fff3dcf63eaf1cf7d14f70a10721026 Reword duplicate error message
* d8ee1b436e4710cb06928e236e89d4330aceab3e Don’t close connection if already closing
* 31bc120bbb6682e02fb2f9f81beff6f132783795 Retry logic for evaluate
* 7ebb70461a4a653a338c46853c6341d253bdaaff Add documents for `calculatepackageid` command
* 3e433d4dbafb4dd97c4a41f0ba7dd45fa9c9e6d4 Add `calculatepackageid` command
* 9ef778ac3dbcb00bcd76eabc85c95418fad1899d Move to better IsAbs Implementation (#3000)
* 0f08904a56477c2407d612fb4dfa0ca261ee2843 Gateway endorsement retry logic
* b4c273174f880b852ddee14e9f633f7d8ba4d559 fix windows SyncDir issue
* c90d50a2e9b661d3a805d13b05750b79332ec597 Bump babel from 2.3.4 to 2.9.1 in /docs
* 0f904bb4f885195797695a453527446b5877dfaa Adjusted from review comments
* 3914549b6ae8781837d2c1085f0174beaa301289 install-fabric.sh script - updated version of bootstrap.
* 3574d8ba88f03f9a9bfda531f455fa25576577a1 Check the package name on core/ledger/kvledger UT (#2987)
* 2ede756b131775954d8397a428765dfda1fc76a5 Extra info in log message (#2982)
* 755ba7974e8190606c7ee3991f951524367e6612 set TestBlockPullerBadBlocks pullblock wait time (#2975)
* b3cf25e84ec731cf955ca1f7dd4218213f61807c Improve health checker docs
* 6897c8005d01772ae5884459c792323675721dc2 Update developer environment (#2977)
* 21e4914ec4011259772ad88b89cdd1927db0488f Rename EndpointError to ErrorDetail (#2974)
* b52f7764203ea65aa9cac6f2b7dfb4d68a18daa9 Add clarifications to dev env versions in doc
* 7d51df1ffbfd99d6bae7899f84bc36c6d082c1f2 docs: Use html_style property instead of add_stylesheet()
* 6656f72563c73a806dee7068dd91b3acf2a286aa Evaluate() error response for node chaincode
* 0625b1063a74b74c930dd12d3652ebf9d896911c Rename persistent_msgs to persistance to avoid protobuf conflict
* c8a6c43b3fa93279972679f50031d8a87562f4f7 Sort chaincode interests in tests (#2966)
* 712458793b9312e8530b7f132332938e6c98c74c Add unittest of writting multiple blocks for `BlockWriter`
* d0b32edae16648230b6efb8b656da26a87b88c34 Add unittest of writting config block synchronously for `BlockWriter`
* 295853bfa7644dbd9326b0bbf12b6a2170a9c659 Write config blocks synchronously in Orderer
* 963633263fe2c0526df64226c700869b22b5f91f Refactor idemix implementation (#2955)
* 4b9ef57ce868febf4993250b6f4a3d6d73a49b62 Fix the project status to 'Graduated' instead of 'Active'
* de9a64dce73b77196a625684103a16e6dde03019 docs: Add the path of softhsm2.conf for macOS
* e66c9514ba40818ed60c53075e956615b591db9f Improve error messages when no endorsers found (#2963)
* c62034e810f51b87a8972ff29a8982085f046023 Add Information about AWS HSM
* 0d13aa6c96efeee2ced8a025d568dd131232e7c2 Update links for Jira to GitHub issue transition in README
* cf341ee49aabae95f583add859ac9186e0a42bb4 Improve an error message in `InstallChaincode`
* 3a936621a66bf866d67901a17317755b7b79eec1 Randomize selection of orderer nodes with retry (#2951)
* 210d20fe4a528793ea12dc5a40ad5d3d9263bc50 Improve wording of log message
* 83cabf287bceecea5b869878ea19a72ab3ac7d08 correct logger labels after cloning block puller.
* f97177c95a5e437a12bbb211d6354850b835befc Cache channel orderers in registry
* f9027a48cb6028243de75240b6a85f90834edaab docs: Don't apply the syntax highlighting of python
* 70ff46ad0181e5e52e25b3566281aa71c05bcdde Unit test flake when rpc server stream not closed (#2935)
* 0545ac8f3ddd607348a91ad07740abc66f23ac42 Fixed Found Typos
* aa8d06b735f82b01ae123e46a0bc21ba831d1b0d Do not create new chain of type etcdraft.Chain if such exists in map of chains. This can happen when in Raft protocol a channel was created, but not marked as done in WAL logs, so at orderer startup it will try to rerun creation tx and panic because the channel already exists.
* 8999ce752abe88ea07a087389ec0bc5f8f7c021f Apply the style only the key in readwrite.rst (#2933)
* 1243e99c1ff249b2c9b9ff6cbcdb05f5f5eceeb5 Fix the result message in test_network.md [ #394 ]
* 8767ceddf604575876be479e77c11d818425e06f Fix broken links for international workgroups (#2920)
* 85a67f833896beb4a86906a876cec13710285198 Implement DisregardNamespacePolicy for gateway
* 3594a3be1644b20bf028fa22f5609a82dfbf0950 Update docs for Jira to GitHub issue transition
* a395f3bcc176441bce6afe2cae4aa8aa2b4876a3 updated chaincode4ade.rst("Writing your first chaincode") showing good practise on how to achieve determinism in json
* b735309e783627a6d530bae15efc69d90f00f57b Updates in main for v2.3.3
* e55a3885f3390c888fd1a6bdfaf1883b4d45e9c2 Minor code clean-up in Gateway ChaincodeEvents handling (#2899)
* beb8f5dacb2fdac0e8ffe6362b1333aacff7f4b2 Implement chaincode event replay for Fabric Gateway (#2896)
* dd539d34970342dd21ce1b7321314faac92958f9 Refactor ChaincodeEvents to use ledger iterator (#2891)
* b1d7538adedaa99bf554138a74360ec4f483baca Private Data Comparison [ #2818 ]
* cbe7d44b1c72d9506a1b41959d7cfcf4b63231ca Nominate Andrew Coleman as Fabric maintainer
* b563b0826ad338177c2fe89d6747355e4a2981c4 Fixed a typo in private_data_tutorial
* 487563520d6d41964602203f29f0caae40dcc07a Update alpine base image to 3.14 (#2881)
* 7cb82eed69f40b8af19bda6e3dd8000dd9a0807b Clean up Go modules (main) (#2878)
* aa76c70591571888d9ad680b7730b0adf922dc0b [Document] typo fix
* 6ec8d727444d59aaf1d36eef010dd2c4fdf8e21f Stop spamming for wait channel acquirement in orderer integration test
* f62e8779d7e898f10e69e84a240a46ac06403c0b Clarify bootstrap.sh message when fabric-samples tag not found
* 868166d7d4b734d9255b31cc6956ed8d1ef952fe Gateway integration tests - adv. endorsement
* 9788c9b3f924543b2a3b72b8480c2f70bfc3a70d Early Differences Flag
* 394fb86ae76b2400422c6b06e34a37808f2dbfca Prepare for next release v2.4.0
* b0e0c4ff29777995d604839a02af98d85b69eccf fix typo
* 1fbdc18bd36e03beb63d078546e201798e62ce50 Update Go to v1.16.7
* 38348fb8a8a1f3024356aba69b4bf8e312391709 [FAB-11334] - Adds a functional / integration test for peer unjoin channel
* bc1898e7db176d2363e983b13afcec3a9754defe Gateway Evaluate() with transient data
* 540fff8b8eed15113bf4e65df43c7a63a644bb37 FAB18529 added nil check in channel header parsing
* 36884f0466344b872c577b4e27bc7f8a54399e5c Add documentation for AbsoluteMaxBytes
* 98973a8f6360bfcad0c79533a7f45bca3d3e1ae0 Options for GRPC message size configurable
* b64d362e24a8f77d5cc18bb2e7b52c4f0b58747e Update bootstrap.sh download script for Fabric CA v1.5.1
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

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=47294&view=logs).</details>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric/releases/tag/v2.4.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-01-28 02:56:11 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.2.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.2.5
                </span>
            </td>
            <td>
                v2.2.5 Release Notes - January 28, 2022
=======================================

Fixes
-----

**orderer - Fix bug when an orderer crashes at channel creation**

This fix handles a scenario where an ordering service node crashes during channel creation.
Previously the ordering service node would attempt to re-create the channel upon next startup,
resulting in a panic with the following error:
"Error creating chain support: error creating consenter for channel: failed to restore persisted raft data: failed to create or read WAL: failed to open WAL: fileutil: file already locked".

**peer - Discovery service does not consider full set of endorsement options**

Due to a bug in the permutation logic, the discovery service may not consider the
full set of endorsement options for a given endorsement policy, potentially resulting in the following error:
"no peer combination can satisfy the endorsement policy".
The fix ensures that all endorsement options are considered for a given endorsement policy and set of peers.


Dependencies
------------
Fabric v2.2.5 has been tested with the following dependencies:
* Go 1.17.5
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
<details><summary><b>See More</b></summary>

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

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=47293&view=logs).</details>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric/releases/tag/v2.2.5" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-01-28 02:57:00 +0000 UTC
    </span>
</div>

