---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.7.0-RC3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.7.0-RC3
                </span>
            </td>
            <td>
                ## 22.7.0-RC3
### Known/Outstanding issues:
- Besu requires a restart post-merge to re-enable remote transaction processing [#3890](https://github.com/hyperledger/besu/issues/3890)
- Investigation/improvement of peering performance is ongoing for post-merge test networks Ropsten and Kiln 

### Additions and Improvements
- Engine API: Change expiration time for JWT tokens to 60s [#4168](https://github.com/hyperledger/besu/pull/4168)
- Sepolia mergeNetSplit block [#4158](https://github.com/hyperledger/besu/pull/4158)
- Goerli TTD [#4160](https://github.com/hyperledger/besu/pull/4160) 
- Several logging improvements 

### Bug Fixes
- fix for stack overflow when searching for TTD block [#4169](https://github.com/hyperledger/besu/pull/4169)
- fix for chain stuck issue [#4175](https://github.com/hyperledger/besu/pull/4175)

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.7.0-RC3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-07-27 17:31:11 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.7.1-RC2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.7.0-RC2
                </span>
            </td>
            <td>
                ### Improvements
- JEMalloc included in this release. jemalloc is an alternative memory allocator that better handles concurrency and memory fragmentation.  Like many other projects, we have discovered that besu benefits from using a modern alternative malloc implementation.  In the latest release we have included a preference for the jemalloc library, and have found it to manage rocksdb memory much more effectively.  In addition to adding this preference in the *nix besu startup script, jemalloc has been baked into our docker images by default. If you are not running docker besu in a docker container,  linux users can leverage jemalloc simply by installing the jemalloc library (which most distributions have a package for)
- RocksDB configuration changes. We have spent time researching how to configure our database technology (RocksDB) to gain better performance and address some recent regressions. We are seeing improvements on Block Import times and memory usage in total, so please update to this build if you are experiencing memory challenges.
- Add a block to the bad blocks if it did not descend from the terminal block [#4080](https://github.com/hyperledger/besu/pull/4080)
- Backward sync exception improvements [#4092](https://github.com/hyperledger/besu/pull/4092)
- Remove block header checks during backward sync, since they will be always performed during block import phase [#4098](https://github.com/hyperledger/besu/pull/4098)
- Optimize the backward sync retry strategy [#4095](https://github.com/hyperledger/besu/pull/4095)

### Bug Fixes
- Changed max message size in the p2p layer to 16.7MB from 10MB to improve peering performance [#4120](https://github.com/hyperledger/besu/pull/4120)
- Fixes for parent stateroot mismatch when using Bonsai storage mode (please report if you encounter this bug on this version) [#4094](https://github.com/hyperledger/besu/pull/4094)
- Above Bonsai related fixes have addressed situations where the event log was not indexed properly [#3921](https://github.com/hyperledger/besu/pull/3921)
- Fixes related to backward sync and reorgs [#4097](https://github.com/hyperledger/besu/pull/4097)
- Checkpoint sync with more merge friendly checkpoint blocks [#4085](https://github.com/hyperledger/besu/pull/4085)
- Fixes around RocksDB performance and memory usage [#4128](https://github.com/hyperledger/besu/pull/4128)
- Fix for RPC performance parallelization to improve RPC performance under heavy load [#3959](https://github.com/hyperledger/besu/pull/3959)
- Fix for post-Merge peering after PoW is removed in our logic for weighting peers [#4116](https://github.com/hyperledger/besu/pull/4116)
- Various logging changes to improve UX- Return the correct latest valid hash in case of bad block when calling engine methods [#4056](https://github.com/hyperledger/besu/pull/4056)
- Add a PoS block header rule to check that the current block is more recent than its parent [#4066](https://github.com/hyperledger/besu/pull/4066)
- Fixed a trie log layer issue on bonsai during reorg [#4069](https://github.com/hyperledger/besu/pull/4069)
- Fix transition protocol schedule to return the pre Merge schedule when reorg pre TTD [#4078](https://github.com/hyperledger/besu/pull/4078)
- Remove hash to sync from the queue only if the sync step succeeds [#4105](https://github.com/hyperledger/besu/pull/4105)
- The build process runs successfully even though the system language is not English [#4102](https://github.com/hyperledger/besu/pull/4102)
- Avoid starting or stopping the BlockPropagationManager more than once [#4122](https://github.com/hyperledger/besu/pull/4122)

### Download links
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.7.0-RC2/besu-22.7.0-RC2.zip / sha256 `d56c340f5982b882fbecca2697ca72a5bbefe0e978d2d4504211f012e2242a81`
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.7.0-RC2/besu-22.7.0-RC2.tar.gz / sha256 `befe15b893820c9c6451a74fd87b41f555ff28561494b3bebadd5da5c7ce25d3`
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.7.0-RC2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-07-20 17:56:48 +0000 UTC
    </span>
</div>

