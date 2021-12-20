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
                PR <a href="https://github.com/hyperledger/besu/pull/3205" class=".btn">#3205</a>
            </td>
            <td>
                <b>
                    CHANGELOG got a bit out of sync. this fixes it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

* Fixes up some alignment issues in the 21.10.x changelog. 
* Adds 21.10.5 
* and removes download link for earlier 21.10.x releases

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-20 03:24:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3204" class=".btn">#3204</a>
            </td>
            <td>
                <b>
                    CI: install a fixed version of solc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

What is currently on main is currently working - but it didn't work when we did release 21.10.4. 
This is the install that was used for release 21.10.4 - is this more reliable?

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-20 03:07:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3203" class=".btn">#3203</a>
            </td>
            <td>
                <b>
                    Update minimum solc version in all contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Recent changes to support latest (0.8.x) version of solc mean that contracts no longer compile with earlier versions. Require at least 0.7.0

Also added SPDX header to some .sol files that were missing it.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-19 22:54:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3202" class=".btn">#3202</a>
            </td>
            <td>
                <b>
                    When downloading the world state, persist children before parents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is still WIP PR. I need to fix tests and make it cleaner. Most of the principles will probably remain for the final PR.

Several changes are happening at the same time in this PR.

1. The pending requests queue in the world state downloader is now a different data structure. We now use a list of priority queues.
2. The node requests now know about the parent request that was responsible for spawning them.
3. When a node has data available and is asked to persist before its children are persisted, the node will not do anything. Instead, it will wait for all its children to persist first and will persist together with the last child. 

Storing children before parents gives us the following benefits:
* We don't need to store pending requests on disk any more. 
* When restarting download from a new pivot, we do not need to walk and check the whole tree any more. 

And the following drawbacks:
* We now have pending nodes in memory for which we already downloaded data, but we do not store them in the database yet. 

Overall expectations on performance:
We still need to download every single state node at least once, so there is no improvement there. We will save a significant amount of time in case we change pivots. And we save lots of read/writes on filesystem because tasks are not needed to be written to disk any more. 

We want to avoid having too many pending unsaved nodes in memory, not to run out of it. If we were always handling only one request to our peers at the same time, we would not need to be worried, and we would just use a simple depth first search. Because we batch our requests, we might produce too many pending unprocessed nodes in memory if we are not careful about the order of processing requests. That is where the priority on node request comes from. We want to always process nodes lower in the tree before nodes higher in the tree, and preferably we want to first process children from the same parent so that we can save the current unsaved parent as soon as possible. 

At the moment, I still left in the code several artefacts that I use for debugging the behaviour. I am planning to get rid of most of these counters, feel free to point them out in the review. There is for instance a weird counter in the NodeDataRequest class that I am using to monitor the total amount of unsaved nodes. In case pending unsaved node count rises too high, there is a warning printed into the logs. At the moment of writing, I would expect the counter to stay below 10 000 generally and not rise above 20 000 nodes. If you saw the number rise to for instance 100 000 that would signify a bug. 

Similarly, because of the order of processing of the nodes, we do not need to store huge number of requests on the disk any more and the whole list fits comfortably into the memory. Without batching, we would not have more than a thousand requests around waiting. Because of the batching, we can see the number of requests occasionally rises all the way up to 300 000, but usually should be under 200 000.

Note that at any time there should not be more pending unsaved blocks than pending requests. Such a situation would be a bug to be reported.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-19 21:20:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3200" class=".btn">#3200</a>
            </td>
            <td>
                <b>
                    Snapshot 21.10.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-19 05:50:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3199" class=".btn">#3199</a>
            </td>
            <td>
                <b>
                    Release 21.10.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-19 05:50:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3198" class=".btn">#3198</a>
            </td>
            <td>
                <b>
                    Update Log4J2 to 2.17.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Security update: upgrade log4j2 to 2.17.0

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-18 16:02:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3197" class=".btn">#3197</a>
            </td>
            <td>
                <b>
                    Bugfix/suggested fee recipient
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
fix a defect found in kintsugi testnet where we produce blocks with the coinbase from miningParams, but use suggestedFeeRecipient for the blockheader.
* consistently use suggestedFeeRecipient and fall back to miningParams
* start MiningCoordinator test coverage with this case
* clean up of unnecessary blockValidator params to MiningCoordinator and BackwardsSyncContext
* ensure only latest (best) blockProposal is available by payloadId from MergeContext

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 18:30:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3196" class=".btn">#3196</a>
            </td>
            <td>
                <b>
                    TEST DO NOT MERGRE Release solc fix
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 00:11:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3195" class=".btn">#3195</a>
            </td>
            <td>
                <b>
                    Fix canDeployContractSignedByPlugin acceptance test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

Fixes `canDeployContractSignedByPlugin` acceptance test by retrieving the transaction hash of the contract deployment programmatically. Removed path for solidity executable to make ot work on MacOS as well.

## Fixed Issue(s)
fixes #3189 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 21:25:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3193" class=".btn">#3193</a>
            </td>
            <td>
                <b>
                    Update CHANGELOG for 22.1.0-RC1 release and prepare it for next RC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 15:44:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3192" class=".btn">#3192</a>
            </td>
            <td>
                <b>
                    Prepare for version 22.1.0-RC2-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 14:58:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3191" class=".btn">#3191</a>
            </td>
            <td>
                <b>
                    Release 22.1.0-RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 14:37:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3186" class=".btn">#3186</a>
            </td>
            <td>
                <b>
                    Validate that blockperiodseconds is set to a positive integer
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

Update ConfigOptions class to validate blockperiodseconds is set to a positive integer when retrieved.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Fixes https://github.com/hyperledger/besu/issues/3093

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 05:34:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3183" class=".btn">#3183</a>
            </td>
            <td>
                <b>
                    install solc in CI; specify solidity version for web3j plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

* install solc on CI executor
* specify version of solidity
* update pragma of all solidity files to allow 0.8 
* two minor changes to solidity so it compiles under solc 0.8

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 03:38:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3179" class=".btn">#3179</a>
            </td>
            <td>
                <b>
                    fastsync refactor for snapsync
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

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-15 17:05:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3178" class=".btn">#3178</a>
            </td>
            <td>
                <b>
                    Revert deletion of the lowest announced block detection
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

Revert deletion of the lowest announced block detection 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-15 15:25:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3177" class=".btn">#3177</a>
            </td>
            <td>
                <b>
                    Make 'to' field optional in eth_call method according to the spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

According to the spec, the 'to' field of a transaction is optional, and it is not specified when call `eth_call` to create a contract.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #3

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-15 12:57:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3176" class=".btn">#3176</a>
            </td>
            <td>
                <b>
                    (fix) log data path on error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span>
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
We will now log the data path if the genesis doesn't match network provided for easier debug

## Fixed Issue(s)
fixes https://github.com/hyperledger/besu/issues/2756

## Changelog
Not required

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-15 02:07:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3175" class=".btn">#3175</a>
            </td>
            <td>
                <b>
                    Update to log4j 2.16.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Updates to log4j2 2.16.0 which identified a second vector for JNDI attacks via `ThreadContext`. Besu only uses `ThreadContext` as part of the acceptance test framework and not in production code so isn't vulnerable to this issue.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 20:46:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3172" class=".btn">#3172</a>
            </td>
            <td>
                <b>
                    factor out timer from BesuRunner into TransactionPoolEvictionService
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

Factor out timer from BesuRunner into TransactionPoolEvictionService so that BesuRunner does not contain inner details of the transaction pool implementation.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 03:57:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3171" class=".btn">#3171</a>
            </td>
            <td>
                <b>
                    Change docker base images from debian to ubuntu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Change the docker base images from debian (implied by openjdk image) to
ubuntu explicitly. Ubuntu has quicker reaction time to base image
security vulnerabilities.

## Fixed Issue(s)

Fixes #3045

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 02:25:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3170" class=".btn">#3170</a>
            </td>
            <td>
                <b>
                    fix comparison in random operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
comparison fix for random operation - compare to UInt256.ZERO rather than Bytes.of(0) when operating in the 'transition' mode between preMergeFork and terminal total difficulty

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 01:14:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3169" class=".btn">#3169</a>
            </td>
            <td>
                <b>
                    Kintsugi v3 fixes
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
* remove MergeBlockImporter, defer to MainnetBlockImporter until there is a specific need to implement a different sync behavior
* fix comparison in RandomOperation


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 01:10:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3168" class=".btn">#3168</a>
            </td>
            <td>
                <b>
                    Fixed typo in option name in CLI dependency check: tls-cipher-suite
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update dependency check for TLS / cipher-suite and added test

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 23:35:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3167" class=".btn">#3167</a>
            </td>
            <td>
                <b>
                    3140 header validation rules
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
Kintsugi header validation rules.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3140

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 22:39:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3166" class=".btn">#3166</a>
            </td>
            <td>
                <b>
                    trace_call API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description
[trace_call API](https://openethereum.github.io/JSONRPC-trace-module#trace_call): Executes the given call and returns a number of possible traces for it.

## Fixed Issue(s)
fixes #2885 

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 15:15:57 +0000 UTC
    </div>
</div>

