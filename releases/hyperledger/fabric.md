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
                    v2.4.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.4.6
                </span>
            </td>
            <td>
                v2.4.6 Release Notes - August 8, 2022
=====================================

Fixes
-----

**orderer - Fix active nodes metric**

Fix active nodes metrics for etcdraft ordering service when a node is evicted.

**peer - Handle malformed gateway request**

If a gateway client sends a malformed request to a peer it may crash the peer node.
This fix checks for the malformed request and returns an error to the gateway client.


Improvements
------------

**Make chaincode-as-a-service (ccaas) builder available in all release distributions**

The chaincode-as-a-service (ccaas) builder executables for `build`, `detect`, and `release` are now available in the Fabric release tar at `builders/ccaas/bin`.


Dependencies
------------
Fabric v2.4.6 has been tested with the following dependencies:
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

* 83596078d0c3d2695dc3bb7bcd726719164adc2c Fix binary package creation
* c9c60fd9be9cac20974f129ef1038881a2b4c2da Release commit for v2.4.6.
* 468332ca3da1d7a37b0b5bcc749d0f4db718e46c Prevent peer from failure on malformed proposal
* 7c12fa69f88218eb2cbca1cb0afccdaf179b89ab Extra checks for invalid args in gateway api
* 84e8b3b22b3e24b71c20d8917dd4cf5a399ede65 fix path for make dir CCAAS Builders
* eb6b172b077c01642c8dc40e84e59ceffcd1bd99 Add -buildvcs=false for ccaasbuilder (#3556) [ #3315 ]
* aa2aaa6b665bba345ebf393744bd795bcce5766f CCAAS Builders
* 0d584c40450b630a904cfa2db9ed9f3330972017 Fixed active nodes metrics for etcdraft when a node is evicted. Instead of being frozen we set it to 0 once halt is called. Tests. (#3536)
* 7e2a6b9ec3347731c80ab09f2ade0dd844f90ed8 Release commit for v2.4.5 (#3505)
* 0f18359493bcbd5f9f9d1a9b05adabfe5da23b06 Check if inner consensus message is missing
<details><summary><b>See More</b></summary>

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
* 9711fb5d0c16297584f5c53123f589110828736f Release commit for v2.4.3
* 47dd17a735118c306c59310fc21f3648e3676e3b Ignore expired CA/TLS CA certs on msp init (#3238) (#3249) (#3252)
* c89ba6048c06ec9ace260733d862112da84f35bb Gateway support for mutual TLS networks (#3235)
* 602f4c6df942faaddb95e153a8c582ed9858b8c5 remove commercial paper references
* 80dbf8ebaff1694ab0ca6c7ebe6bca4513be17a2 Add Intermediate CA certs to dial options (#3225) (#3226)
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

This list of changes was [auto generated](https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=55501&view=logs).</details>
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric/releases/tag/v2.4.6" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-08-08 21:49:18 +0000 UTC
    </span>
</div>

