---
layout: default
title: indy-plenum
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/indy-plenum
---

# indy-plenum <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-plenum){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.13.1-rc1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.13.1-rc1
                </span>
            </td>
            <td>
                [v1.13.1-rc1] 

## What's Changed
* Check test suit preparation exit code by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/547
* [INDY-1019] sdk integration by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/525
* reset last_ordered_3PC for future views during view change. by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/548
* fix KeyError for "services" when pool ledger contains node update txns by @lovesh in https://github.com/hyperledger/indy-plenum/pull/549
* INDY-1112: change primeries election procedure for backup instances. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/539
* INDY-1113: Node disconnection, view change tests by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/551
* [INDY-1165] Try to decrease testing time by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/552
* [INDY-1148] It's possible to create several nodes with the same alias by @Toktar in https://github.com/hyperledger/indy-plenum/pull/554
* [INDY-1171] Integrate pool_transactions tests with libindy by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/541
* [INDY-993] Test_batch_rejection integrated with sdk by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/558
* INDY-1148 : change test for validation nodes txns by @Toktar in https://github.com/hyperledger/indy-plenum/pull/560
* [INDY-988] testRequestDynamicValidation sdk integration by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/557
* [INDY-994] Logging tests sdk integration by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/559
* [INDY-1102] Fix Logger setting by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/555
* [INDY-1186] Added prefix REPLICA with name for replica logging by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/565
* [INDY-1185] Fixing build on hyperledger jenkins by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/553
* [INDY-1001] Move plenum/test/instances tests to sdk by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/563
* Context manager for delay rules in stasher by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/566
* Send ledger status to new nodes in all cases; test for node restart by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/567
* [INDY-1138] Added ppTime for stateTsDbStorage by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/569
* Test restart nides by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/571
* [INDY-1138] Added get_equal_or_prev into parent class by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/570
* Fix none finalised reqs in case of not participating by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/574
* [INDY-1137] Making proof possible for given root hash by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/575
* [INDY-992] Move bls tests to sdk by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/564
* [INDY-1180] Do not raise error if commit for previous view by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/578
* INDY-1205: Use RocksDB as a key-value storage by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/561
* [INDY-1058] Get rid of Registry-based pools by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/568
* Indy 1180 fix none finalised by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/581
* INDY-1205: rename get_equal_or_prev test. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/580
* INDY-1205: fallback to leveldb by default for db hash storage. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/584
* INDY-1205: add build procedure of rocksdb package to build-3rd-partie… by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/583
* Use leveldb for the ledger by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/585
* INDY-1205: add maintainer to rocksdb deb package. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/586
* Fixed test genesis txns by @Toktar in https://github.com/hyperledger/indy-plenum/pull/587
* Remove test repo from CI docker. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/589
* INDY-1205: make ledger default storage configurable. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/590
* [INDY-1206] select_primaries now called after poolLedger catchup or if we are ordering node txn by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/588
* Tests unusual behaviour fix by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/591
* [INDY-1187] Implement log processor by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/573
* Downgraded severity of some messages from debug to trace by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/592
* Log processor improvements by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/593
* [INDY-1210] Added resending instance change messages by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/594
* [INDY-1238] Limit zmq queue with 10000 msgs by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/597
* Improve request tracking in log processor by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/596
* [INDY-1209] Raise node_request and pool_transactions fixtures and helper functions by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/579
* refactoring and new tests by @lovesh in https://github.com/hyperledger/indy-plenum/pull/598
* [FIX TESTS] Fix consistency proof query test by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/608
* Trying to fix testAddInactiveNodeThenActivate by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/606
* add min, max length support to iterables by @lovesh in https://github.com/hyperledger/indy-plenum/pull/612
* Fix for Base58key test by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/611
* Fixed memory leak in monitoring by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/613
* [INDY-1225] Implemented compression, increased log rotation interval by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/607
* Log processor: improvements in request tracking and statistics by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/601
* INDY-1259: fix typo. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/615
* Fixed log rotation config by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/614
* [Increment sdk] Increment libindy and python wrappers version by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/616
* [pool-refresh-fix] Handle CommonIOError by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/621
* Public/indy 1265 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/622
* New libindy 454 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/628
* [INDY-465] Warning and callback on unordered requests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/619
* Log processor: improved request tracking by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/617
* Add pip version and bump indy-crypto by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/632
* Log processor: faster filtering by timestamp by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/634
* [INDY-1237] Get rid of RegistryPoolManager by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/595
* [INDY-1173] add POOL_RESTART handling by @Toktar in https://github.com/hyperledger/indy-plenum/pull/582
* [Fixed failed tests] Decrease reconnect timeout and ensure the same data by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/637
* Log processor: minor fixes by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/636
* Added Copyright to plenum license by @vimmerru in https://github.com/hyperledger/indy-plenum/pull/639
* INDY-1251: change math of spikes detection. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/640
* INDY-1287: fix base58 version by @Toktar in https://github.com/hyperledger/indy-plenum/pull/644
* Log processor: track COMMIT messages by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/642
* INDY-1237: Fix tests that used nodeRegistry. by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/643
* [1209-1] Remove old client's fucntions by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/600
* Indy 1256 propagare primary by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/641
* INDY-1292: fix base58 version in build scripts by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/648
* INDY-971: Added state diagrams for catch-up actors by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/630
* [Decrease base58] Decrease base58 to "editable" 0.2.4 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/649
* [INDY-1291] Freeze deps packages version by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/650
* switches pr context to hyperledger by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/652
* [INDY-1291] Remove dublicate orderedset building by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/651
* [FIX 3rd parties] Remove dublicate again by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/653
* Jsonpickle version by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/656
* INDY-1261: add flushing of retry count per remote by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/655
* [INDY-1200] Each next 3PC batch have a timestamp not less than the previous one by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/646
* INDY-1251: fix data in notifier plugin tests and unskip them. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/647
* [Pygment fix] Bump pygment version and remove version for leveldb by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/658
* INDY-1287: fix base58 version 1.0.0 by @Toktar in https://github.com/hyperledger/indy-plenum/pull/645
* [Pygments] bump pegments into setup.py by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/659
* [Pygments] Add patch version for pygments by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/661
* INDY-1289: support read-only mode for rocksdb and leveldb. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/660
* [INDY-1175] Extend validator information by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/599
* Fixed flakiness in test_request_time_tracker by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/662
* INDY-1244: set RocksDB as a key-value storage for all. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/665
* [INDY-1274] Add log information for unordered txn by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/663
* INDY-1273/1275: Log rotation improvements by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/657
* INDY-1274: log level fix by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/667
* [RUN_CMD] Catch stderr if external cmd flush error into stderr (jouralctl inside docker containers for example) by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/666
* [INDY-1289] Added read_only for ledger by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/669
* INDY-1173: add DatetimeStringField by @Toktar in https://github.com/hyperledger/indy-plenum/pull/670
* [Bump indy-crypto] Bump indy-crypto and python3-indy by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/672
* Log processor: fixed edge case by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/671
* [INDY-1175] Stay "Metrics" as a dict by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/674
* INDY-1297 / INDY-1298: Corrected catch-up logic by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/638
* Indy 1175 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/677
* INDY-1251: improve logging of spike detection. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/676
* INDY-1274: Fix for logging by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/675
* INDY-1290: Design for implementing PBFT view change in indy plenum  by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/673
* INDY-1316:  bug with end greater then catchupTill in processCatchupReq by @Toktar in https://github.com/hyperledger/indy-plenum/pull/680
* INDY-1236: solve problem with excess message requests with prepare and preprepare by @Toktar in https://github.com/hyperledger/indy-plenum/pull/664
* INDY-1349: Implement configurable periodic view change by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/686
* INDY-1316: added check to discard in test_incorrect_catchup_request by @Toktar in https://github.com/hyperledger/indy-plenum/pull/684
* [INDY-1175] Fixes for vaildator-info by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/681
* INDY-1319: fix test_request_executed_once_and_without_failing_behind. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/687
* [INDY-1175] fix upgrade_log reading by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/688
* Fix tests. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/689
* Remove strange test and incorrect helper. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/691
* Txn refactoring by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/695
* INDY-1319: return get() method back to the ledger implementation. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/696
* Fix flake errors by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/697
* INDY-1329: Short checkpoint and lag for catch-up by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/690
* INDY-1304: Implement tests that show problems with current view change by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/693
* [WiP] INDY-1304: Added view change tests for Case 4 by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/703
* Patricia trie prefix proof support by @lovesh in https://github.com/hyperledger/indy-plenum/pull/694
* INDY-1319: move calculation of seqNo's from ledger's appendTxns(). by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/702
* INDY-1304: Added tests that show problems with current view change [test #3] by @Toktar in https://github.com/hyperledger/indy-plenum/pull/701
* INDY-1319: remove apply() method from ConfigReqHandler class. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/706
* INDY-1304: Tests refactoring by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/705
* INDY-1329: Removal of previous stashed checkpoints by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/704
* INDY-1332: support binding of client and node listeners on different … by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/707
* [INDY-1319] txn-refactoring for update node txn through old cli by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/709
* [INDY-1319] Replace txn with txn_data by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/710
* [INDY-1319] fix flake8 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/711
* Txn format refactoring by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/683
* [WiP] INDY-1304: Added view change tests for Case 5 by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/708
* INDY-1332: support different queue sizes for nstack and cstack. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/715
* INDY-1332: support node/client IPs in test network setup. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/716
* State proof optimisation by @lovesh in https://github.com/hyperledger/indy-plenum/pull/700
* fix missing seq_no in test genesis txns by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/719
* INDY-1332: set 0.0.0.0 for node and client IPs for test network setup. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/722
* [INDY-1327] change key-value in ReqIdrToTxn  by @Toktar in https://github.com/hyperledger/indy-plenum/pull/712
* INDY-1341: Increase viewchange/catchup timeout to 5 minutes by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/717
* [txnId_Fix] Add txn_id while metadata appending (if exist) by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/724
* INDY-1327: add method get_protocol_version()  for seqNoDB migration by @Toktar in https://github.com/hyperledger/indy-plenum/pull/727
* [Remove alias] Remove alias from genesis transactions generating by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/728
* INDY-1393: Add optional field PROTOCOL_VERSION to LEDGER_STATUS by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/730
* [WIP][INDY-1370] Сhange key in requests map by @Toktar in https://github.com/hyperledger/indy-plenum/pull/713
* Recorder by @lovesh in https://github.com/hyperledger/indy-plenum/pull/692
* [INDY-1370]: fix expectingAcksFor and expectingRepliesFor maps key by @Toktar in https://github.com/hyperledger/indy-plenum/pull/735
* Bump protocol_version by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/734
* [INDY-1369] Bump minor version for indy-plenum by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/736
* Intermittent test by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/732
* change reqId in replayer by @lovesh in https://github.com/hyperledger/indy-plenum/pull/739
* abstract comparison logic to a method and return small values as comp… by @lovesh in https://github.com/hyperledger/indy-plenum/pull/740
* [INDY-810] Review and replace assert where needed [common,  crypto, ledger, plenum/plenum] by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/726
* INDY-1245: support RocksDB storage configuration. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/731
* Patch 102 by @lovesh in https://github.com/hyperledger/indy-plenum/pull/742
* Reduce log rotation backup count by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/746
* INDY-1410: Fixed bug with KeyError by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/743
* INDY-1373: Support running log processor on headless systems by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/745
* [INDY-810] Review and replace assert in state, storage, stp_core and stp_zmq by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/748
* INDY-1390: reduce MAX_RECONNECT_RETRY_ON_SAME_SOCKET from 5 to 1. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/749
* New sdk by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/741
* Add progress info to output of replay by @devin-fisher in https://github.com/hyperledger/indy-plenum/pull/752
* Add missed txnId to txn in ledger by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/755
* Adds exception handling for 3pc msgs processing by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/758
* fix signature scheme name by @lovesh in https://github.com/hyperledger/indy-plenum/pull/759
* INDY-1393: Add PROTOCOL_VERSION validation by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/733
* Fix nym path to make it str by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/760
* INDY-1405: Apply stashed batches taking into account that they can be already partially commited by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/747
* [INDY-1387] Change config's params for stability by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/737
* fix for failing test by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/765
* [log exception] log if unhandled exception was raised by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/764
* Hotfix for node crash by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/768
* [Remove tb] remove tb printing in wrap method by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/769
* use protocolVersion=1 in test genesis files by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/770
* use protocolVersion=None in test genesis files by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/772
* payment plugin changes by @lovesh in https://github.com/hyperledger/indy-plenum/pull/774
* fix get value from state if there is no BLS multi-sig by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/778
* Fixes and improves metadata routine by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/776
* minor refactor by @jerrysen in https://github.com/hyperledger/indy-plenum/pull/780
* rename plenum_config.py to indy_config.py by @lovesh in https://github.com/hyperledger/indy-plenum/pull/744
* fix stasher by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/782
* INDY-1404: Do not do view change until catchup is finished by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/757
* Public/indy 1417 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/784
* Correct spelling of checkpoints in validator-info output by @ckochenower in https://github.com/hyperledger/indy-plenum/pull/787
* INDY-1422,1429: Hot fixes by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/785
* [ci skip] Adds ability to set pr context for cd pipeline from environment variable by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/792
* [INDY-1385] Fix last_prepared_sertificate computing by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/786
* INDY-1427: Fix bug in stashed checkpoints removal by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/791
* fix restart tests to use a correct timeout for check connections by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/789
* Fixes in tests and monitor by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/793
* INDY-1386: clear requests list after view change for ordered txns by @Toktar in https://github.com/hyperledger/indy-plenum/pull/781
* INDY-1453: do not process client reqs during View Change by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/796
* INDY-1452: store seqNo-3PCKey map for ledgers after catchup by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/795
* INDY-1458: do not start propagate primary if view change is in progress by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/798
* [INDY-1435] Throughput calculating fixes by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/797
* Log messages modification to reduce total size by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/794
* add test for delayed IC and VCD during view change by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/803
* INDY-1454: Fix perpetual catchup during view change by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/804
* INDY-1431: implement client stack restart on reached connections limit. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/799
* Log processor: add support for new log format by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/806
* Extend logging with checkpoint send by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/805
* INDY-1450: Request ledger statuses and consistency proofs in catchup by @Toktar in https://github.com/hyperledger/indy-plenum/pull/800
* INDY-1464: fix Propagate request for ATTRIB txn by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/807
* INDY-1467: get rid of peersWithoutRemotes. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/808
* INDY-1454: Reset timeout when starting consecutive view change by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/802
* Trying to fix some flaky tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/810
* New stack sizes: clien 3k, node 20k by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/813
* [INDY-1462] Set H as maxsize for backup replicas if propagating primary (for new joined node) by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/809
* INDY-1461: add the test for different prepare certificates in view change by @Toktar in https://github.com/hyperledger/indy-plenum/pull/815
* INDY-1484: Fix flaky test by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/817
* INDY-1487: Fix flaky tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/818
* INDY-1447: Fixed handling of forced requests by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/819
* INDY-1199: Implement inconsistent 3PC state detection by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/811
* make schema non-strict by default by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/816
* [INDY-1471] Fixes logger initialization inside Cli constructor by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/821
* INDY-1447: Made minor corrections by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/822
* [Bump version] bump version to 1.5 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/823
* [INDY-1470] Add fix for received instance_change from unknown node by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/820
* [INDY-1468] move avgLatency computing to EMA algorithm by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/812
* INDY-1486: Attempt to fix intermittent test by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/828
* INDY-1199: Improve integration tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/826
* INDY-1496: enable client stack restart by default. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/830
* INDY-1502: Improve log rotation logic by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/831
* Add get_utc_datetime utility by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/832
* Must return a 4-tuple from consume_req_queue_for_pre_prepare by @ckochenower in https://github.com/hyperledger/indy-plenum/pull/833
* Add config for initial propose viewchange timeout by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/827
* INDY-1507: Fix rare failure case by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/834
* INDY-1477: fix discard calling if node is blacklisted. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/835
* INDY-1431: add listener bind retries. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/838
* INDY-1475: Implement metrics gathering by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/837
* INDY-1519: Fixed handling of message replies by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/841
* [INDY-1468] Fix metrics displaying by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/842
* [INDY-1478] Fix CurrentState building and FutureViewChangeDone logic by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/836
* INDY-1475: Preparation for statistics processing script by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/843
* INDY-1531: add bind-before-connect to control outgoing routing. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/845
* INDY-1475: Implement calculating metrics dynamics by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/846
* New sdk version by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/814
* INDY-1475: Fix losing events with same timestamps  by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/847
* INDY-1497: Fix sending to not connected remotes by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/849
* INDY-1497: Fix sending to not connected remotes by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/844
* [INDY-1542] Validator additionals by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/848
* INDY-1475: Metrics improvements by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/850
* INDY-1544: Fix for INSTANCE_CHANGE sending by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/851
* INDY-1549: Change default settings for better performance and stability by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/853
* Adjust node parameters by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/855
* Plenum 683 by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/856
* INDY-1543: Add more metrics by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/857
* INDY-1545: stop processing checkpoints in view change by @Toktar in https://github.com/hyperledger/indy-plenum/pull/854
* INDY-1545: fix condition of discard checkpoints in processing by @Toktar in https://github.com/hyperledger/indy-plenum/pull/859
* [INDY-1555] Add monitor reseting after view_change complete and disab… by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/858
* upgrade plenum version to 1.6 by @Toktar in https://github.com/hyperledger/indy-plenum/pull/860
* INDY-1543: Fix crash in get_metrics by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/863
* Log processor improvements by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/862
* INDY-1564: Discard any client requests during view change by @Toktar in https://github.com/hyperledger/indy-plenum/pull/866
* get request handler by txn type by @lovesh in https://github.com/hyperledger/indy-plenum/pull/869
* Public/indy 1562 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/868
* INDY-1199: Enable inconsistency watchdog based on network events by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/873
* [INDY-1587] Add size limitation for listener reading and set quotas for node and client stacks separately by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/874
* INDY-1543: Metrics improvements by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/870
* [INDY-1582] add median for calculating average throughput and latency for backups by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/871
* INDY-1543: Make metrics flush interval configurable by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/875
* INDY-1543: Fix crash in stddev, add average bounds by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/877
* [INDY-1389] Support Proof of Possession for BLS keys by @Toktar in https://github.com/hyperledger/indy-plenum/pull/867
* INDY-1583: Removal of check for pre-prepare by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/878
* INDY-1564: Fix problem with incorrect Nack response message. by @Toktar in https://github.com/hyperledger/indy-plenum/pull/876
* INDY-1389: added check to case with bls key proof without key by @Toktar in https://github.com/hyperledger/indy-plenum/pull/880
* [INDY-1595] change batch building by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/879
* Remove memory profiler from default validator info params by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/881
* Validator info changes by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/883
* [Size experiments] increase size for client and node stacks by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/884
* INDY-1602: Add more metrics by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/882
* INDY-1588: Add method for generating key proof by @Toktar in https://github.com/hyperledger/indy-plenum/pull/886
* Rename properties to make them public by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/887
* INDY-1602: Add more metrics, remove some by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/888
* INDY-1602: Metrics improvements by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/889
* Update Jenkins CI config by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/893
* INDY-1583: Fix bls signature checking  by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/890
* INDY-1565: Throughput measurement strategies by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/872
* INDY-1639: First implementation of accumulating strategy by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/891
* INDY-1602: Quotas, metrics by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/896
* Minor fix in monitor by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/898
* INDY-1645: Fix for config dependencies bug by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/900
* INDY-1659: Improve performance of monitor by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/902
* [INDY-1642] Discarded field to bitmask by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/895
* [INDY-1642] Move discarded to list of invalid indices by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/903
* Public/indy 1642 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/906
* Public/indy 1642 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/907
* INDY-1602: Dynamic quota control by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/905
* accept threshold param in authenticate by @lovesh in https://github.com/hyperledger/indy-plenum/pull/908
* INDY-1589: A node be able to participate in BLS multi-signature only if it has a valid proof of possession by @Toktar in https://github.com/hyperledger/indy-plenum/pull/901
* INDY-1621: Fix for adding node with existing HAs by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/904
* INDY-1637: add optional RocksDB usage for ValidatorInfo class. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/910
* INDY-1580: Resolve prepare and commits missing problem by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/894
* Indy 1599 from aw by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/914
* [INDY-1599] Add strategies for latency measurement by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/892
* INDY-1673: Changes to reply pre_send hook. by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/915
* INDY-1680: add function for removing replica by @Toktar in https://github.com/hyperledger/indy-plenum/pull/912
* INDY-1657: Enhanced logging of state changes by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/916
* INDY-1700: Removing rejected reqs from Propagator by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/920
* INDY-1602: Add more metrics by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/921
* [INDY-1649] Do not re-authenticate Propagate messages by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/919
* INDY-1649: do not re-verify signature for Propagates. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/911
* [INDY-1649] fix verified_reqs cleaning by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/923
* INDY-1688: Fix requests tracking in monitor by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/924
* [INDY-1649] clean verified reqs only for instance of ReqAuthenticator by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/926
* Additional collections metrics by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/929
* INDY-1681: Backup replica removal on primary loss by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/925
* INDY-1681: Fixed bug with missed super() reference by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/931
* INDY-1740: Fixed a bug in re-asking cancellation by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/933
* INDY-1719: Fixes for node demotion/promotion by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/922
* Corrected level matcher in process_logs by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/928
* Metrics improvements by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/934
* INDY-1739: Eliminated concurrent catchups by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/939
* INDY-1719: Fix for node demotion by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/935
* INDY-1711: Bugfix in  LedgerManager._processCatchupReplies by @Toktar in https://github.com/hyperledger/indy-plenum/pull/936
* [INDY-1649] Checnge tests for checking auth call count by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/930
* Reduce frequency of writes into metrics_db by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/941
* INDY-1739: Unit tests for ability to start catchup by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/943
* [bump indy-crypto] bump version for python3-indy-crypto by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/944
* INDY-1723: Profiling on node objects  by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/945
* Remove memory dump, add new kv storage metrics by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/946
* Validator info dump time revert by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/947
* INDY-1765: Add cleaning requestQueue in Replica in the method _gc() by @Toktar in https://github.com/hyperledger/indy-plenum/pull/950
* INDY-1753: Eliminated request schema re-validation by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/953
* INDY-1682: Remove replicas then instance performance degraded by @Toktar in https://github.com/hyperledger/indy-plenum/pull/948
* Fix intermittent tests by @Toktar in https://github.com/hyperledger/indy-plenum/pull/955
* File storage support for testing purposes by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/952
* INDY-1775: add CONNECTED_CLIENTS_NUM metric. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/956
* Return last view change strategy for primary performance degradation by @Toktar in https://github.com/hyperledger/indy-plenum/pull/960
* Add logs to accumulating monitor strategy by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/961
* Warn if looper iteration is too long by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/962
* INDY-1795: Resume ordering on backup replica by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/964
* INDY-1682: bugfix in  logic for instance performance degraded by @Toktar in https://github.com/hyperledger/indy-plenum/pull/963
* Remove ret val declaration by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/965
* INDY-1683: bugfix backup_instance_faulty_processor with quorum logic by @Toktar in https://github.com/hyperledger/indy-plenum/pull/954
* [INDY-1687] Add strategy for getting node-to-node messages before view_change by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/958
* INDY-1815: areBackupsDegraded() are not use latency anymore by @Toktar in https://github.com/hyperledger/indy-plenum/pull/967
* Add GC-related metrics by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/968
* Change TolerateBackupPrimaryDisconnection to 180 sec by @Toktar in https://github.com/hyperledger/indy-plenum/pull/969
* [INDY-1687] small changes in tests by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/970
* [INDY-1687] Add logs and some comments by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/972
* INDY-209: Fix init_indy_node script by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/966
* Add GC-related metrics by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/976
* INDY-209: Additional formatting by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/975
* [INDY-1835] Enable PreViewChange strategy by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/977
* INDY-1780: add draft implementation of dropping of outdated requests. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/973
* [INDY-1849] fix for each message serialization during batch handling by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/978
* Fix memory leak by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/979
* Add public/private key exception handling by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/981
* INDY-1759: Restoration of lastPrePrepareSeqNo by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/971
* INDY-209: Additional formatting by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/982
* [INDY-1849] Call send method from ZStack class during resending stashed to disconnected by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/985
* use latest stable libindy by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/987
* INDY-1851: Plenum consensus protocol diagram by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/989
* [INDY-1770] Decrease MAX_CONNECTED_CLIENTS_NUM to 400 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/988
* INDY-903: Removal of client codebase by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/986
* INDY-1846: Change pool state root hash for BLS-signature in Commit messages by @Toktar in https://github.com/hyperledger/indy-plenum/pull/980
* Fix and improve documentation by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/993
* INDY-1872:L fix replica removing tests by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/992
* INDY-1846: add more logging in bls signature validation by @Toktar in https://github.com/hyperledger/indy-plenum/pull/994
* Fix rare flakiness of test_metrics_config by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/991
* INDY-1869: Catch-up procedure sequence diagram by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/996
* Improve measure_time metrics tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/998
* INDY-1868, 18709: Adding more diagrams by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/997
* INDY-1770: decrease clients connections limit. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/1000
* INDY-1870: Update storages.md by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/999
* Fixing Documentation by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1001
* Add bls, ip to default validator info; software info now generates on… by @dsurnin in https://github.com/hyperledger/indy-plenum/pull/995
* INDY-1869: Catch-up procedure sequence diagram by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/1003
* INDY-1843: Discard pre-prepare with ordered request by @Toktar in https://github.com/hyperledger/indy-plenum/pull/990
* Add more metrics by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1006
* INDY-1872: fix bug in create_throughput_measurement by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1005
* Old client's lump removal by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1009
* Client removal fixes by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1011
* INDY-1882: Checkpoints feature sequence diagram by @spivachuk in https://github.com/hyperledger/indy-plenum/pull/1007
* INDY-1836: add test for request drop on propagate phase. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/984
* INDY-1881: Catchup clearing by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1004
* INDY-1866: Fix memory leak by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1012
* INDY-1836: enable clear request queue strategy by default. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/1013
* INDY-1898: add statistics for outdated requests. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/1014
* INDY-1836: fix removing of entries from requests queue. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/1015
* INDY-1836: add unit tests for requests drop. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/1018
* INDY-1896: Allow "read" and "action" requests processing by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1016
* Improve reporting of objects tracked by GC by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1019
* INDY-1896: Add test to read requests in view change and refactoring for client requests discarding by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1021
* INDY-1879: faster way for pool transactions ordering by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1010
* INDY-1883: add documentation for Message Requests by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1027
* INDY-1856: Defining new PoA interfaces  by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1030
* INDY-1836: increase ToleratePrimaryDisconnection and bind re-try time. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/1029
* INDY-1856: Fix validator info init by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1031
* INDY-1902: add a doc with known ZMQ features. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/1032
* INDY-1909: add discarding of old instance change messages  by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1028
* INDY-1836: clear monitor data related to dropped request. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/1033
* INDY-1911: add integration tests  by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1034
* INDY-1926: add check for None of replica's primary name during logging. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/1039
* INDY-1925: Fixes for documentation by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1040
* INDY-1836: add test of req drop when replica does not order. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/1042
* INDY-1836: add force_free() method for Requests. by @sergey-shilov in https://github.com/hyperledger/indy-plenum/pull/1043
* INDY-1924: Catchup and audit design proposal by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1044
* INDY-1856: Implementation of new req_handlers by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1038
* Fix intermittent tests by increasing timeouts by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1048
* [pytest] pin pytest-asyncio version to 0.8.0 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1049
* Enable readthedocs support by @michaeldboyd in https://github.com/hyperledger/indy-plenum/pull/1037
* INDY-1924: Add options concerning BLS multisigs by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1051
* INDY-1922: Fix and tests for crop upgrade log by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1050
* [INDY-1876] Integration ReplicaStasher and ReplicaValidator by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1046
* INDY-933: Support regular freshness update of BLS state by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1047
* INDY-1876: Change order of stashing by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1053
* INDY-1858: Fix in node_handler and tests by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1052
* INDY-1949: Add more logging by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1056
* INDY-1949: a test reproducing the problem by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1057
* INDY-933: Improve docstring, reduce flakiness of some tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1054
* Additional metrics for stashed requests by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1059
* [INDY-1928] Add freshness info into validator-info output by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1058
* [INDY-1928] add some fix into replayable node by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1060
* INDY-1955: fixing infinite catch-up by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1061
* INDY-1949: Modify logging, remove redundant validation by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1064
* [WIP]INDY-1874 General Tracker  by @cam-parra in https://github.com/hyperledger/indy-plenum/pull/1062
* INDY-1955: don't send CatchupReq to disconnected and unresponsive nodes by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1063
* Fix confition for dequeueing of stashed commits by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1065
* [INDY-1957] Adds Identity Owner to enum of possible roles by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1068
* INDY-1955: add REPLICA_STASH_LIMIT to config by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1067
* Add test_dequeue_and_validate_commits by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1066
* INDY-1965: move logs about stash messages to TRACE by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1069
* INDY-1965: Delay propagate request. Optimization. by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1071
* [INDY-1874] changes in uncommitted tracker by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1072
* Indy 1874 Improved logic for tracker and more tests by @cam-parra in https://github.com/hyperledger/indy-plenum/pull/1070
* INDY-1965: Review fixes by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1074
* INDY-1917: Fixes for correct replicas addition by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1076
* INDY-1965: Logging changes by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1077
* INDY-1911: Send INSTANCE_CHANGE when state signatures are not fresh enough by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1078
* INDY-1966: add on_strategy_complete to VCStartMsgStrategy by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1081
* INDY-1933: Fix for backup throughput measuring by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1080
* INDY-1956: Default config changes by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1083
* [INDY-1874] changes to ledger_uncommitted tracker by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1084
* INDY-1754: add test_random_string for randomString by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1086
* INDY-1911: Make acceptable freshness interval configurable by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1085
* Fixes fpm installation for build env by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1089
* Extract ViewChangeDataProvider by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1088
* Refactoring test_twice_demoted_node_dont_write_txns by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1082
* [INDY-1874] add set_last_committed and delay_without_unstash for tests by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1092
* INDY-1984: Persiste INSTANCE_CHANGE messages between restarts by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1087
* Implement and use new timers in ViewChanger by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1093
* INDY-1720: Test reproducing problem by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1090
* [INDY-2001] move write_req_validator into node init by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1094
* INDY-1944: Audit ledger support by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1091
* Simulation test for ViewChanger by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1095
* INDY-2008: Fix a problem with view change and add audit ledger in validator-info by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1097
* INDY-1944: Audit ledger txn format fixes by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1100
* INDY-1945: Implement NodeSeederService by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1098
* INDY-2003: add parameter can_be_empty in LimitedLengthStringField by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1102
* INDY-1945: Integrate SeederServices into LedgerManager by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1101
* Set fixed version of jenkins shared library for CD pipeline by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1103
* INDY-1945: Add __init__.py to plenum/server/catchup by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1104
* [INDY-2006] add no_wait option for sdk_add_new_nym by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1105
* INDY-1961: Audit ledger documentation by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1106
* INDY-1945: Implement CatchupRepGatherer by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1108
* [INDY-1992] Adds base classes to support versioning routine by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1110
* INDY-1945: Extract routing from RxChannel by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1111
* [INDY-1995] add metric for collecting count of using auth rules from … by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1112
* INDY-1945: Integrate CatchupRepGatherer into LedgerManager by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1109
* INDY-1945: LedgerInfo cleanups by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1113
* INDY-1944: Сheck audit txn root when validating prepare by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1107
* INDY-1945: Move logic into ConsProofService by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1114
* INDY-1945: Integrate ConsProofService into LedgerManager by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1115
* [INDY-1992] versioning and release changes by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1116
* [INDY-1992] Makes metadata unambiguous for CD pipeline by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1119
* INDY-1945: Implement LedgerLeecherService by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1117
* INDY-1945: Integrate LedgerLeecherService into LedgerManager by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1118
* [INDY-2020] fixes imports of 'packaging' module by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1122
* INDY-1945: Implement NodeLeecherService by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1120
* [WIP][INDY-2010] add command GET_AUTH_RULE by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1121
* [INDY-2003] remove isSteward from modern reg_handlers by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1124
* INDY-2010: fix a reply format for domain transactions by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1126
* INDY-1945: Fix catchup logic to use audit ledger by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1123
* [WIP] INDY-1945: Cleanups + parallel catchup by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1127
* Fix filling InstanceChanges from database in InstanceChangeProvider by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1128
* INDY-1961: Update docs regarding cacthup process by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1129
* INDY-1945: Minor catchup improvements by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1130
* INDY-1993: Hotfix for crash in generating consistency proof by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1132
* Catchup log messages improvements by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1133
* INDY-1993: Move catchup start notification before consistency proof gathering by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1134
* [ST-513] add txn_root into LedgerUncommittedTracker by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1135
* INDY-2018: Fix node verkey validation by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1137
* INDY-1993: improve logging; correctly set last committed after catchup of audit by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1138
* INDY-2022: Fix last_ordered_3pc catching up by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1140
* INDY-1993: Catchup tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1136
* INDY-2022: Review fixes by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1141
* [Malicious_primary] fix count of request for reverting by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1142
* [INDY-1992] new release logic activation by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1125
* INDY-1946: Restore current 3PC state from audit ledger [skip ci] by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1096
* INDY-1946: Fix for replicas inconsistency by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1147
* INDY-2032: extend logging by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1146
* INDY-2025: Fix some catchup problems by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1149
* ST-541 Add flag to disable seqNoDB update during catchup by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1148
* INDY-2032: Fix phantom transactions in audit ledger by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1151
* ST-528: add the POST_NODE_STOPPED hook by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1152
* bump libindy by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1157
* bump libindy by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1139
* [ST-520] add unregister_req_handler method with unit tests by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1158
* ST-541 Fix creation of audit ledger transactions by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1154
* INDY-1757: Double digest validation implemented by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1150
* [INDY-1983] Tracking PP first validation time to check their obsolescences by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1155
* INDY-2047: Make initial catchup without audit ledger more robust by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1159
* [INDY-1983] fixes wrong comment by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1160
* INDY-1674: Plugin's field included in digest by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1162
* INDY-2025: Improve tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1156
* INDY-1863: Allow limiting maximum number of 3PC batches in flight by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1163
* INDY-2043: Add validation of 'signature' and 'signatures' in authenticate() method by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1164
* INDY-2050: remove LogicError from  __is_next_pre_prepare by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1167
* INDY-2046: View change only on master malicious by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1168
* INDY-2055: Make changes in txn metadata format backward compatible by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1165
* Fix addition of new ledger  by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1170
* INDY-2043: change LimitedLengthStringField format by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1171
* INDY-2051: Payload digest fix by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1172
* New tests and docs update by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1166
* INDY-2050: test for view change with missing PrePrepares  by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1175
* INDY-2056: Handle gracefully some corner cases by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1176
* INDY-2060: Fix a problem with watermarks after ViewChange by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1174
* Adjusts CD pipeline for jenkins lib v2.0.4  by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1181
* Bumps jenkins lib version to 2.0.5 by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1186
* Fix crash when catching up genesis txns by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1187
* Do not check freshness in a catchup. by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1179
* ST-549 Fix Request for requests without identifier by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1188
* INDY-2053: Implement new CATCHUP_REQ distribution logic by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1173
* INDY-1863: Set default Max3PCBatchesInFlight to 4 by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1189
* Bumps version to 1.8.0.dev0 by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1190
* ST-549 Fix signature creation for requests without identifier by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1192
* INDY-2053: Improve catchup logging by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1193
* [INDY-2072] Requests with taa by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1191
* INDY-2053: Fix one more edge case in catch up by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1194
* Use master build of libindy by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1197
* INDY-2066: Implement TXN_AUTHOR_AGREEMENT transaction by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1196
* INDY-2066: Refactor and add tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1199
* INDY-2066: Fix tests to use libindy by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1200
* INDY-2066: Make ts store support different ledgers by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1201
* INDY-2066: Improve tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1202
* [INDY-2066] Adds more taa data to state by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1203
* INDY-2067: Implement GET_TXN_AUTHOR_AGREEMENT by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1204
* INDY-2068: TAA AML txn implementation, tests by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1205
* ST-557 Add taaAcceptance field to Request builder by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1207
* INDY-2067: Implement getting TAA by timestamp, improve tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1206
* [INDY-2073] Dynamic validation for client requests taa acceptance data by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1195
* INDY-2067: Validate parameters combinations in GET_TAA by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1208
* Support empty TAA by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1210
* TAA AML tests improvements by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1209
* Reduce amount of logged information by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1211
* [INDY-2073] TAA Acceptance validation: stricter logic and sdk integration in tests by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1213
* INDY-2071: GET_TAA_AML txn implementation by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1212
* [INDY-2073] Minor fixes by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1214
* INDY-2074: Transaction Author Agreement Docs by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1216
* [INDY-2105] Updates for docker used in debs build routine by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1217
* [INDY-2109] Bumps jenkins library version to 2.1.1 by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1218
* Upgrade plenum version to 1.9 by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1226
* INDY-2122: Don't send NACK for requests discarded during view change by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1223
* INDY-2087: Bump libindy version to 1.9.0-dev-1122 by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1225
* INDY-2129: Fix the problem with demoting a backup primary node by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1227
* INDY-2097: update pluggable request handlers by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1221
* [INDY-1860] node's bootstrap with pluggable request handlers by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1222
* INDY-2087: bump libindy version by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1233
* ST-510 Add request param for write request handler by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1236
* INDY-2097: Update pluggable request handlers  by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1234
* INDY-2098: Improve tests for TAA state proofs by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1228
* INDY-2083: Try asking for cons proofs without timeout by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1235
* INDY-2108: More tests for pluggable request handlers by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1232
* [INDY-1860] move init to separate helper class by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1237
* INDY-2108: Write request manager tests by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1238
* INDY-2108: Add unit tests for pluggable request handlers by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1240
* Improves pipelines by @andkononykhin in https://github.com/hyperledger/indy-plenum/pull/1241
* [WIP][INDY-1861] Pluggable request handlers integration by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1239
* INDY-1338: View change design updates and Plenum 2.0 Architcture diagrams by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1244
* INDY-1338: Design interfaces for ViewChangeService + PoC simulation tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1242
* INDY-2144: Fix validation for forced requests by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1243
* ST-523: Fix for plugins integration by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1249
* INDY-2153 Fix external audit requests by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1250
* Test for audit txn sending by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1251
* ST-601 Remove 32-bytes length check from removal to be compliant with… by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1248
* INDY-2135: Simulation tests for PBFT View Change protocol by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1246
* [INDY-2163] move to new docker images with changed gpg keys by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1257
* [INDY-2154] remove old req handlers by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1247
* [BUMP] bump jenkins shared to 2.2.1 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1259
* INDY-2157: TAA acceptance use date by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1256
* INDY-2157: change the reject message for a too precise TAA time in requests by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1263
* INDY-2147: Stashing router + example usage by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1264
* INDY-2147: Improve StashingRouter by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1265
* INDY-2147: Implement PBFT view change by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1267
* INDY-2139: Extract and integrate ConsensusDataProvider by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1262
* INDY-2147: Fixes in PBFT View Change Math by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1268
* INDY-2164: add re-sending failed msgs for clients by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1260
* INDY-2112: make reask_ledger_status() and _reask_last_cons_proof() repeatable by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1269
* [INDY-2136] First stage for OredringService by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1266
* INDY-2143: Fix for additional instance_change by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1270
* Bump libindy 1167 by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1271
* Fix for provider by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1272
* INDY-2157: bump sdk version, add a TAA integration test by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1273
* INDY-2157: bump libindy version by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1277
* INDY-2147: Added more unit tests for View Change Service by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1274
* Bump indy-plenum version to 1.9.1 by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1278
* INDY-2171: Signature verification changes by @ArtObr in https://github.com/hyperledger/indy-plenum/pull/1276
* [INDY-2136] PR's review by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1275
* INDY-2173: Support Transaction Endorser field in Request by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1281
* INDY-2173: support Endorser field in Request by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1282
* INDY-2162: bump libindy by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1288
* INDY-2137: Extract CheckpointService from Replica by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1279
* ST-601 -- add randomized test for removal of keys from the state by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1261
* INDY-2179: Integrate CheckpointService to Replica by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1289
* Bump plenum version to 1.9.2 by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1291
* INDY-1335: use BatchID instead of PrePrepares in consensus shared data by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1292
* Change a log level for messages from the ClientMessageProvider by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1293
* INDY-2167: Integrated PrimarySelector into View Change Service by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1290
* Fixes for Python 3.6 support by @andrewwhitehead in https://github.com/hyperledger/indy-plenum/pull/957
* INDY-2200: Use production req handlers in simulation tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1294
* INDY-2169: Integrate OrderingService into Replica by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1280
* INDY-2169: Allow to unsubscribe from event buses by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1298
* [INDY-2169] additions for indy-node and plugins by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1299
* INDY-2177: Use audit txn root hash as checkpoint digest by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1296
* INDY-1335: View Change fixes and improvements by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1297
* INDY-2208: Integration of Services: Cleanup by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1300
* Increase ZMQ bind retry timeout by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1302
* INDY-1954 -- Implement GET_TXN audit proof read by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1303
* INDY-2215: add re-ask LedgerStatuses for the init catchup by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1305
* INDY-1954 Add multisig check by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1308
* [INDY-2218] Add check for identifier decoding by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1309
* INDY-2208: add an internal_bus to each replica by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1310
* INDY-2177: Rework CheckpointerService internals by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1304
* INDY-2208: remove ConsensusDataHelper, hooks by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1312
* [1.10.0] bump package version to 1.10.0 by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1316
* Add CODEOWNERS by @ryjones in https://github.com/hyperledger/indy-plenum/pull/1307
* Modify Codeowners list by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1319
* Change the formatting of exceptions for the client by @donqui in https://github.com/hyperledger/indy-plenum/pull/1318
* [INDY-2103] Minor changes to how exception formating is done by @donqui in https://github.com/hyperledger/indy-plenum/pull/1320
* INDY-2183: Increase frequency of re-connection checks by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1315
* SN-7: move init states from ledger after Node initialization by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1321
* SN-7: fix KeyValueStorageInMemory by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1324
* [INDY-1336] Stop dropping ppSeqNo to 0 after view_change by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1301
* [INDY-2177] Merge "stop dropping pp_seq_no" changes by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1323
* [WIP] INDY-1340: Checkpointer cleanups by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1317
* INDY-1340: pp_view_no (original view no) support by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1326
* [INDY-2177] ToDo in tests by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1327
* INDY-1340: request missing old view PrePrepares when applying NewView by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1329
* INDY-2220: add and integrate MessageReq3pcService by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1306
* ST-623 -- Init Commit multi-sig process by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1325
* [INDY_2149] Add test with real ordering by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1328
* INDY-1340: go to next view on timeuout for PBFT View Change Service by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1330
* [INDY-1336] Reset pp_seq_no for backup after view_change by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1331
* [INDY-2223] Fix reordering after view_change by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1334
* INDY-2178: Request missing ViewChange messages by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1335
* INDY-2222 -- improve logging by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1337
* INDY-2223: Improve simulation tests by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1333
* INDY-2172: Changed the log level for removed RIDs by @donqui in https://github.com/hyperledger/indy-plenum/pull/1340
* INDY-2223: ViewChange message serialization by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1338
* INDY-2222 -- Add some more logs by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1339
* [INDY-2223] First step in view_change integration by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1341
* INDY-2178 Integrate ViewChange messages requesting to ViewChangeService by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1342
* INDY-2223: Fix test_view_change_with_next_primary_stopped by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1344
* [INDY-2213]: Bump pyzmq version by @donqui in https://github.com/hyperledger/indy-plenum/pull/1348
* [INDY-2223] Issues with reordering after vc and tests by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1347
* INDY-2223: add more sim tests by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1349
* [INDY-2213]: Fix FPM dependencies by @donqui in https://github.com/hyperledger/indy-plenum/pull/1350
* INDY-2223: Switch to PBFT view change  by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1345
* INDY-2223: fix message stashing in view change by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1353
* INDY-2233 -- Fix audit proof for GET_TXN by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1356
* INDY-2223: reset monitor after reOrdering by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1355
* INDY-2140: Cleanup old view change logic by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1357
* INDY-2140: Cleanup old view change logic by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1360
* INDY-2140: add prepared and preprepared lists cleaning by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1361
* INDY-2231: fixing checkpoint stabilization after view change on nodes lagging behind by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1359
* [INDY-2140] Fix tests in view_change directory by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1366
* [FUTURE RELEASE] bump devs version by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1365
* INDY-2222 -- reconnection fix by @KitHat in https://github.com/hyperledger/indy-plenum/pull/1363
* INDY-2140: update node_state after view change by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1364
* [INDY-2230] do not send NewView msg if primary is behind by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1368
* INDY-2140: Sync finishing view change on backups and master + more cleanups by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1362
* INDY-2140: remove state logic from FuturePrimariesBatchHandler by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1367
* INDY-2248: add a message validation for instance id by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1372
* [INDY-2140] Stabilize checkpoints on backups after view change by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1370
* Change logging for select primary by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1374
* Add default SECURITY policy by @ryjones in https://github.com/hyperledger/indy-plenum/pull/1352
* [INDY-2213]: Update pyzmq for Jenkins CD by @donqui in https://github.com/hyperledger/indy-plenum/pull/1351
* INDY-2140: Get rid of legacy view change completion check by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1371
* INDY-2224: Request `NewView` from a Primary. by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1375
* INDY-2253: do not stash ping/pong for reconnection nodes when sending… by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1376
* INDY-2244: optimize finalized requests logic by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1377
* INDY-2244: New flags to disable batching and message requests by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1378
* INDY-2247: propose view change if a new primary is same with a previous one by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1379
* INDY-2023: remove an outdated test by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1382
* [INDY-2235]: Save (pre)prepares in audit ledger by @donqui in https://github.com/hyperledger/indy-plenum/pull/1383
* Indy 2261: do not send ping/pong msgs in Batches  by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1384
* INDY-2274: add ROUTER_HANDOVER option by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1386
* [INDY-2235]: Improving tests by @donqui in https://github.com/hyperledger/indy-plenum/pull/1385
* INDY-2268: increment Max3PCBatchWait by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1388
* INDY-2261: Add options to not use custom reconnect logic by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1387
* [INDY-2244] Cleanup and fix primaries adding by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1381
* [Future release] bump package version by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1391
* [INDY-2267] remove primaryChange and simplify catchup_complete logic by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1392
* INDY-2262: Implementing NodeRegHandler  by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1397
* LGTM Recommendation fixes by @donqui in https://github.com/hyperledger/indy-plenum/pull/1399
* INDY-2262: fix revert and cleanup of node_reg_at_beginning_of_view  by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1400
* INDY-2262: send InstanceChange for every node count changing by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1395
* INDY-2262: use NodeRegHandler for Primary Selection by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1398
* [INDY-2236] Forcing VC by qourum of ViewChange msgs by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1401
* [INDY-2292] change State restoring logiс by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1402
* INDY-2292: fix restore_state() in WriteRequestManager by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1403
* INDY-2263: Make ViewChangeService unsubscribe from messages on cleanup by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1404
* INDY-2262: fix restoring node reg for Ordered if it's not in audit ledger yet by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1408
* INDY-2292: add more tests for a state restoring by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1407
* INDY-2298: do not restore primaries from the audit ledger  by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1406
* INDY-2262: fix filling node reg in audit ledger by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1410
* INDY-2262: fix node reg in audit ledger  by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1412
* Fix passing connections to services by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1413
* INDY-2285: change digest format for PrePrepare by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1411
* INDY-2292: restore state with versioning by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1419
* [FUTURE_RELEASE] bump dev version by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1421
* [INDY-2286] Add NODE txn handling into simulation tests by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1409
* [INDY-2289]: ZMQ auto reonnect fixes by @donqui in https://github.com/hyperledger/indy-plenum/pull/1422
* INDY-2280: Do not sign and verify BLS signature twice by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1423
* INDY-2280:  do not deserialize BLS public key on every signature verification by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1425
* INDY-2263: Implement ViewChangeTriggerService and PrimaryConnectionMonitorService by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1405
* [WIP][INDY-2289]: Handling messages delivered pre-catchup by @donqui in https://github.com/hyperledger/indy-plenum/pull/1426
* [INDY-2294] Turn off transport batches by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1427
* [INDY-2289]: Additional tests by @donqui in https://github.com/hyperledger/indy-plenum/pull/1428
* [INDY_2306]: Remove size limit for outbound msgs by @donqui in https://github.com/hyperledger/indy-plenum/pull/1429
* [INDY-2024] remove steward-only check for NODE txns by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1430
* INDY-2297, INDY-2302: Allow multiple active TAAs, change GET_TAA's reply format  by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1424
* INDY-2302/2313: Update Transaction Author Agreement documentation by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1432
* [CI] increase timeout for CI by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1433
* INDY-2313: Update TAA-related namings by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1434
* INDY-2138: add a documentation for a new PBFT View Change by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1431
* INDY-2316 Allow multiple active TAAs: Debug by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1436
* [INDY-2299] Stop ordering on backup while master is in reordering stage. by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1435
* INDY-2316: bugfix in update_state for txn_author_agreement_handler by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1438
* INDY-2316: fix for getting txn version for a state recovering by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1439
* INDY-2313: Require ratification_ts to create TAA by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1437
* INDY-2316: disable only active TAAs by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1442
* INDY-2316: fix TxnAuthorAgreementDisableHandler by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1443
* INDY-2313: Minor updates to TAA and view change docs by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1440
* INDY-2316: Improve integration tests, fix unretirement edge case by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1444
* INDY-2316: bump libindy version, use taa request builder from libindy by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1448
* Add test_view_change_permutations by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1449
* INDY-2318: remove code for re-sending to disconnected  by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1441
* [FUTURE_RELEASE] bump dev version by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1450
* INDY-2319: use committed node reg when selecting Primaries for the next view by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1447
* [INDY-2314] make LimitedLengthStringField length 256 by default by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1451
* [INDY-2324] Get requestQueues back after reverting by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1453
* INDY-2324: Move remaining parts of legacy ViewChanger into new services by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1454
* INDY-2324: Remove legacy view changer by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1457
* [INDY-2308] Allow NEW_VIEW processing from other nodes and finish view_change by quorum of them by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1458
* INDY-2322: Fix Primary Selection and N calculation logic by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1456
* [INDY-2324] Get back requests from PrePrepare by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1461
* [INDY-2308] Added additional test and fix for another edge-case by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1460
* INDY-2324: Improvements in SimNetwork by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1459
* INDY-2326: consider node_reg at the end of last view as the one at the beginning of current view by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1464
* INDY-2326: Use uncommitted node reg at the beginning of view to select primaries in audit ledger by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1465
* [INDY-2324] Add random initial view no for sim pool by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1455
* [FUTURE_RELEASE] bump package version by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1468
* [INDY-2326] Add test for restarting only after promotion by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1469
* [INDY-2326] add another demotion/promotion tests and fix by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1470
* [INDY-2330] Tool for checking zmq connection by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1471
* [INDY-2330] Move to pypi by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1472
* INDY-2338: support generic way for request payload version by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1473
* [ERROR_HANDLING] add module with examples for Exception handling by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1474
* [ERROR HANDLING] Document error handling strategies by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1476
* Support error codes for TAA errors  by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1475
* fix InvalidClientMessageException str representation by @ashcherbakov in https://github.com/hyperledger/indy-plenum/pull/1477
* Change a string format for InvalidClientMessageException by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1478
* [FIX] fix client-related behaviour by @anikitinDSR in https://github.com/hyperledger/indy-plenum/pull/1479
* Some changes needed for Ubuntu 20.04 support by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1480
* INDY-2311: Ursa support in plenum by @skhoroshavin in https://github.com/hyperledger/indy-plenum/pull/1481
* Add validations for TAA_ACCEPTANCE_TIME and timestamps in the TAA txn by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1483
* Update link in README.md by @MrMaavin in https://github.com/hyperledger/indy-plenum/pull/1489
* FIX #1495 Missing ursa in build script for generating .deb by @georgepadayatti in https://github.com/hyperledger/indy-plenum/pull/1496
* Fix CVE-2019-18874 by @dhh1128 in https://github.com/hyperledger/indy-plenum/pull/1498
* Fixing CD by @askolesov in https://github.com/hyperledger/indy-plenum/pull/1499
* Fixed Jenkinsfile.cd by @askolesov in https://github.com/hyperledger/indy-plenum/pull/1500
* Fix link to transactions.md page by @Patrik-Stas in https://github.com/hyperledger/indy-plenum/pull/1482
* Fixing CD pipeline by @askolesov in https://github.com/hyperledger/indy-plenum/pull/1501
* WIP:  Ubuntu 20.04 VM setup by @ryMarsh44 in https://github.com/hyperledger/indy-plenum/pull/1508
* [UP-34]: add LEDGERS_FREEZE and GET_FROZEN_LEDGERS transactions by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1502
* Bump libindy ver 1.15.0~1618 by @adenishchenko in https://github.com/hyperledger/indy-plenum/pull/1510
* GitHub actions CI workflow by @WadeBarnes in https://github.com/hyperledger/indy-plenum/pull/1513
* Update CODEOWNERS by @askolesov in https://github.com/hyperledger/indy-plenum/pull/1518
* Publish tests report steps are now allowed to fail by @askolesov in https://github.com/hyperledger/indy-plenum/pull/1523
* Add settings file. by @ryjones in https://github.com/hyperledger/indy-plenum/pull/1521
* Github actions CD steps for plenum by @ianco in https://github.com/hyperledger/indy-plenum/pull/1519
* Add doc for freeze ledger by @adenishchenko in https://github.com/hyperledger/indy-plenum/pull/1511
* Split CD release into two parts, added caching, and extended Docker file by @udosson in https://github.com/hyperledger/indy-plenum/pull/1526
* Skip problem seeds for view change simulation tests.  by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1525
* check if record.message exists with hasattr or use record.msg by @devinleighsmith in https://github.com/hyperledger/indy-plenum/pull/1528
* UP-34: bump libindy, use ledgers_freeze from libindy for tests by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1520
* Merge Stable to Master by @Toktar in https://github.com/hyperledger/indy-plenum/pull/1515
* Upgrade Ubuntu 20.04 by @adenishchenko in https://github.com/hyperledger/indy-plenum/pull/1522
* Update runner to be compatible with python 3.8, pytest 6.2.2 by @devinleighsmith in https://github.com/hyperledger/indy-plenum/pull/1530
* Remove some pinned dependencies by @adenishchenko in https://github.com/hyperledger/indy-plenum/pull/1534
* Ubuntu 20.04 pull master by @adenishchenko in https://github.com/hyperledger/indy-plenum/pull/1532
* Ubuntu 20.04: fix Libindy version  by @adenishchenko in https://github.com/hyperledger/indy-plenum/pull/1539
* Ubuntu 20.04: remove pip imports in favor if importlib_metadata by @udosson in https://github.com/hyperledger/indy-plenum/pull/1550
* Ubuntu 20.04: Publishing artifacts (debian packages) by @udosson in https://github.com/hyperledger/indy-plenum/pull/1545
* set publishPackages as executable by @udosson in https://github.com/hyperledger/indy-plenum/pull/1558
* Support publishing off a development branch by @WadeBarnes in https://github.com/hyperledger/indy-plenum/pull/1557
* Ubuntu 20.04: Publishing of Python packages to PyPI by @udosson in https://github.com/hyperledger/indy-plenum/pull/1559
* Bug fix: Cache of 3rd party dependencies & uploading of existing packages to PyPI  by @udosson in https://github.com/hyperledger/indy-plenum/pull/1561
* Remove unused dockerfiles by @WadeBarnes in https://github.com/hyperledger/indy-plenum/pull/1560
* Ubtuntu 20.04: fix uploading of deb files with the same name but different distribution by @udosson in https://github.com/hyperledger/indy-plenum/pull/1566
* updated version of setup-jfrog-cli to v2 by @udosson in https://github.com/hyperledger/indy-plenum/pull/1574
* added versions of 3rd party packages to Debian artifacts by @udosson in https://github.com/hyperledger/indy-plenum/pull/1576
* pinned version of importlib-metadata because of issue with fpm by @udosson in https://github.com/hyperledger/indy-plenum/pull/1577
* Devcontainers by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1580
* fixed typo in gitpodlink by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1582
* Build-indy-plenum-docker and 3rd parties switched to the GHA Dockerfile by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1583
* Removal of Jenkins files Fixes #1553 by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1584
* removed pip legacy resolver in gitpod.yml due to being deprecated by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1586
* GHA Refactoring by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1585
* Enforce LF for VScode by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1587
* Upgrade zmq by @WadeBarnes in https://github.com/hyperledger/indy-plenum/pull/1589
* New Release Workflow by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1590
* Fixes #1592 & removal of old build scripts by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1593
* Pinned indy-shared-gha reference by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1595
* Addition of StatusCheck for branch protection by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1596
* Added CICD Documentation reference by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1594
* Adjust workflow triggers. by @WadeBarnes in https://github.com/hyperledger/indy-plenum/pull/1598
* [v1.13.1rc0] - Update Version Number for Release by @sovbot in https://github.com/hyperledger/indy-plenum/pull/1599
* fixed GHA variable format errors by @pSchlarb in https://github.com/hyperledger/indy-plenum/pull/1600
* [v1.13.1-rc1] - Update Version Number for Release by @sovbot in https://github.com/hyperledger/indy-plenum/pull/1601

## New Contributors
* @vimmerru made their first contribution in https://github.com/hyperledger/indy-plenum/pull/639
* @jerrysen made their first contribution in https://github.com/hyperledger/indy-plenum/pull/780
* @ckochenower made their first contribution in https://github.com/hyperledger/indy-plenum/pull/787
* @michaeldboyd made their first contribution in https://github.com/hyperledger/indy-plenum/pull/1037
* @cam-parra made their first contribution in https://github.com/hyperledger/indy-plenum/pull/1062
* @KitHat made their first contribution in https://github.com/hyperledger/indy-plenum/pull/1148
* @ryjones made their first contribution in https://github.com/hyperledger/indy-plenum/pull/1307
* @donqui made their first contribution in https://github.com/hyperledger/indy-plenum/pull/1318
* @MrMaavin made their first contribution in https://github.com/hyperledger/indy-plenum/pull/1489
* @georgepadayatti made their first contribution in https://github.com/hyperledger/indy-plenum/pull/1496
* @askolesov made their first contribution in https://github.com/hyperledger/indy-plenum/pull/1499
* @Patrik-Stas made their first contribution in https://github.com/hyperledger/indy-plenum/pull/1482
* @ianco made their first contribution in https://github.com/hyperledger/indy-plenum/pull/1519
* @devinleighsmith made their first contribution in https://github.com/hyperledger/indy-plenum/pull/1528
* @pSchlarb made their first contribution in https://github.com/hyperledger/indy-plenum/pull/1580

**Full Changelog**: https://github.com/hyperledger/indy-plenum/commits/v1.13.1-rc1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/indy-plenum/releases/tag/v1.13.1-rc1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-06-03 17:24:49 +0000 UTC
    </span>
</div>

