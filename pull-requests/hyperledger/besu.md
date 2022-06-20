---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3995" class=".btn">#3995</a>
            </td>
            <td>
                <b>
                    snap persist progress 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 13:16:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3994" class=".btn">#3994</a>
            </td>
            <td>
                <b>
                    When on PoS the head can be only be updated by ForkchoiceUpdate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When executing a newPayload or build a new block, we do not need to move
the chain head and update the world state, since this will be done by a
following forkchoice update call, but we still need to validate the block
and doing so we can also prepare everything for the future call, so we do
not need to re-execute everything, but only update the pointers, so that the
response to the forkchoice update call is quick.

Moreover on block proposal do only a validation of the block without storing or remembering nothing, to avoid saving data that could be stale, for example the empty block that is always proposed, is useless if another better block is produced later.
Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3957
## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 12:58:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3993" class=".btn">#3993</a>
            </td>
            <td>
                <b>
                    Additional testings on ignored option warning 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                ## PR description
Add tests on options configured through ENV

## Fixed Issue(s)
Follow-up PR to address comments from https://github.com/hyperledger/besu/pull/3969 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 05:16:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3992" class=".btn">#3992</a>
            </td>
            <td>
                <b>
                    Added ARM tasks to CI config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mark-terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Added ARM CircleCI tasks to verify compatibility.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 01:37:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3989" class=".btn">#3989</a>
            </td>
            <td>
                <b>
                    issue #3986 -  Changed [file path init fail error message] clearer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Error message when the data path is not accessible was not clearly describing the actual error. So I made this error message more intuitive.    

## Fixed Issue(s)
fixes #3986 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 17:15:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3985" class=".btn">#3985</a>
            </td>
            <td>
                <b>
                    Apply some RocksDB documentation suggestions to reduce memory usage.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Apply some [RocksDB documentation suggestions](https://github.com/facebook/rocksdb/wiki/Memory-usage-in-RocksDB) to reduce memory usage.

- Set format_version to 5
- set optimize_filters_for_memory to true
- Increase block size to 32K
- set cache_index_and_filter_blocks to true 

There is almost 1,5 GiB difference in memory consumption between this version and version 22.4.2 on a 16 GB RAM VM after 1 day of syncing (the green line represents the metrics of this PR). 

<img width="824" alt="Screenshot 2022-06-17 at 10 27 59" src="https://user-images.githubusercontent.com/5099602/174259124-fa8d8eef-fa51-424e-96f3-3a3d3bc71b07.png">

Sync time is equivalent between the two versions.

<img width="1620" alt="Screenshot 2022-06-17 at 10 35 02" src="https://user-images.githubusercontent.com/5099602/174260539-792ae296-8bef-42f0-b47d-94a08ec3271c.png">

Disk usage, CPU consumption and the number of open file descriptors is quite similar for tho instances.

<img width="815" alt="Screenshot 2022-06-17 at 10 30 44" src="https://user-images.githubusercontent.com/5099602/174259784-e458ec70-7cfc-4f87-a587-4f4375915d4a.png">
<img width="1624" alt="Screenshot 2022-06-17 at 10 30 59" src="https://user-images.githubusercontent.com/5099602/174259780-1052143e-a5b2-492e-8805-7b4ed56542df.png">
<img width="816" alt="Screenshot 2022-06-17 at 10 31 18" src="https://user-images.githubusercontent.com/5099602/174259775-0d1e536c-6751-46de-b923-fa2ae1486749.png">




Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 08:36:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3984" class=".btn">#3984</a>
            </td>
            <td>
                <b>
                    DO NOT MERGE - Spike external db
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Please do not merge.

This is a spike for the storing the chain data in an external db instead of the local rocksdb database. I've only made this a draft PR so I more easily create builds for testing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 05:44:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3983" class=".btn">#3983</a>
            </td>
            <td>
                <b>
                    update the docker container versions for Tessera and GoQuorum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                On my new M1 mac book the Tessera docker wouldn't start. Updating the Tessera docker version fixed that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 02:24:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3979" class=".btn">#3979</a>
            </td>
            <td>
                <b>
                    updates version to prep for q3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 18:34:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3978" class=".btn">#3978</a>
            </td>
            <td>
                <b>
                    Release 22.4.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                reverts PR for disconnecting from the pow network. Updates version number.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 17:09:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3977" class=".btn">#3977</a>
            </td>
            <td>
                <b>
                    Thread Safe Bonsai World State Updater Facade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Recent problems with world state mismatch on bonsai are most probably caused by synchronization issues.

Bonsai data structure is not inherently tread safe as compared to how forest works. 

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 14:48:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3976" class=".btn">#3976</a>
            </td>
            <td>
                <b>
                    adds ttd block to sepolia config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 13:50:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3975" class=".btn">#3975</a>
            </td>
            <td>
                <b>
                    Remove check in fcU if new blocks are descendants of the previous finalized block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## Fixed Issue(s)
fixes #3966 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 13:47:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3974" class=".btn">#3974</a>
            </td>
            <td>
                <b>
                    fix ThreadBesuNodeRunner missing engineRpcConfiguration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Acceptance test fail to run with `ThreadBesuNodeRunner` when `systemProperty 'acctests.runBesuAsProcess = false'`. This PR adds missing configurations to ThreadBesuRunner for engine RPC API. 



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Failure Example:
```
./gradlew acceptanceTest --tests="*ExecutionEngine*"

Cannot parse null string
java.lang.NumberFormatException: Cannot parse null string
	at java.base/java.lang.Integer.parseInt(Integer.java:630)
	at java.base/java.lang.Integer.valueOf(Integer.java:999)
	at org.hyperledger.besu.tests.acceptance.dsl.node.BesuNode.getEngineJsonRpcPort(BesuNode.java:372)
	at org.hyperledger.besu.tests.acceptance.dsl.node.BesuNode.engineRpcUrl(BesuNode.java:309)
	at org.hyperledger.besu.tests.acceptance.jsonrpc.ExecutionEngineAcceptanceTest.test(ExecutionEngineAcceptanceTest.java:83)
```

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 13:26:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3973" class=".btn">#3973</a>
            </td>
            <td>
                <b>
                    adds websocket methods, test coverage still lacking
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #3948 

Signed-off-by: Justin Florentine <justin+github@florentine.us>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 12:51:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3972" class=".btn">#3972</a>
            </td>
            <td>
                <b>
                    set merge flag false for tests that need it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Since we currently have a static config object, if tests are run in a different order or in parallel, this can break the tests. Quick fix - set the flag to false for the tests that got broke.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 05:43:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3970" class=".btn">#3970</a>
            </td>
            <td>
                <b>
                    WIP: fixing the sonarcloud building in gha
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Joshua Fernandes <joshua.fernandes@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 00:59:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3969" class=".btn">#3969</a>
            </td>
            <td>
                <b>
                    Have consistent warning between CLI, ENV and TOML config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add additional check of option in environment variables and config file for detecting ignored dependent config warning.

## Fixed Issue(s)
fixes #2069 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 00:30:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3967" class=".btn">#3967</a>
            </td>
            <td>
                <b>
                    Create sonarcloud.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Joshua Fernandes <joshua.fernandes@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Adding in sonarcloud via Github Actions

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 21:24:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3965" class=".btn">#3965</a>
            </td>
            <td>
                <b>
                    init optional and logging fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 15:41:20 +0000 UTC
    </div>
</div>

