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
                PR <a href="https://github.com/hyperledger/besu/pull/4190" class=".btn">#4190</a>
            </td>
            <td>
                <b>
                    Feature/engine api override
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
Allow besu to have the engine api enabled, when there are not merge configs.  includes:
* un-hiding/un-deprecating `--engine-rpc-enabled`
* remove old isMergeEnabled checks in a few block header validators
* use merge-specific block header validator, rather than appending to MainnetBlockHeaderValidator

Tested with Hive and Kurtosis since this affects block validation.  Both are 🟢 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4172 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 04:48:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4189" class=".btn">#4189</a>
            </td>
            <td>
                <b>
                    Accept empty header set in range headers validation
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

If a response to the get header P2P request only returns the header that
is the start of the range we may need to trim it to an empty response,
this is breaking the validation response. One client has started
returning only the range header start in some circumstances (which is a
valid response per spec). Because we sometimes request an overlapping
header this results in an empty stream once we cut the duplicates.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

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
        Created At 2022-07-28 04:33:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4186" class=".btn">#4186</a>
            </td>
            <td>
                <b>
                    Only stop block propagation, not tx handling.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Since there is a Subscribers for each type of message handler in EthMessages, and only on handler, they all get a subscriber id of 1.  This changes the unsubscribe logic to require the caller to specify the message code handler being unsubscribed from, and removes it from the map of handlers.

## Fixed Issue(s)
fixes #3890 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 22:48:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4185" class=".btn">#4185</a>
            </td>
            <td>
                <b>
                    Switching info to trace on several noisey logs during sync.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: matt-nelson-csi <matt.nelson@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
Fixes #4182 - switches info to trace on the three noisy Sync commands 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 21:55:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4181" class=".btn">#4181</a>
            </td>
            <td>
                <b>
                    Prepare for version 22.7.0-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare for version 22.7.0-SNAPSHOT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 17:57:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4180" class=".btn">#4180</a>
            </td>
            <td>
                <b>
                    Release 22.7.0-RC3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.7.0-RC3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 17:14:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4179" class=".btn">#4179</a>
            </td>
            <td>
                <b>
                    fix enr request order
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
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
        Created At 2022-07-27 13:22:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4178" class=".btn">#4178</a>
            </td>
            <td>
                <b>
                    DNS peers handled the same as boot nodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Peers discovered through the DNSDaemon are now added to the peerTable. These peers are potentially used (16 are randomly chosen from the peer table) in RecursivePeerRefreshStateas as the initial peers for bonding and then for finding neighbours, etc.

Signed-off-by: Stefan <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 12:28:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4177" class=".btn">#4177</a>
            </td>
            <td>
                <b>
                    Allow to set any value for baseFeePerGas in the genesis file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also made baseFeeFloor final.

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Even if not pratical on mainnet or main testnes, in theory in the genesis file, the `baseFeePerGas` field could be set to any Wei value, for example it could be 1 Wei, as done in the Hive test `consensus/checkGasLimit_London`.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes  Hive test `consensus/checkGasLimit_London`

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 11:54:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4175" class=".btn">#4175</a>
            </td>
            <td>
                <b>
                    Add mechanism to retrieve missing blocks 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@consensys.net>

## PR description
Add mechanism to retrieve missing blocks when a pending block is saved

## Fixed Issue(s)
#3955

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 00:12:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4174" class=".btn">#4174</a>
            </td>
            <td>
                <b>
                    Add ZeroBaseFeeMarket to support post-London free gas networks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows private networks already using London fee market to start using free gas. Previously, since https://github.com/hyperledger/besu/pull/4003, it was only possible to start a free gas London network from genesis.

Details on https://github.com/hyperledger/besu/issues/4061

Fixes https://github.com/hyperledger/besu/issues/4061

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 22:53:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4173" class=".btn">#4173</a>
            </td>
            <td>
                <b>
                    Print warning for deprecated testnets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Prints a deprecation warning for Ropsten, Kiln and Rinkeby

## Fixed Issue(s)
fixes #4163

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

The documentation should mention that Ropsten, Rinkeby and Kiln are deprecated

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 22:03:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4171" class=".btn">#4171</a>
            </td>
            <td>
                <b>
                    4169 dont recurse
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

Replaces recursive implementation of isDescendentOf with a loop.

## Fixed Issue(s)
fixes #4169 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 18:30:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4170" class=".btn">#4170</a>
            </td>
            <td>
                <b>
                    Fixed desired gas limit setting in the reference tests service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
FIxes #4167 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 15:47:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4168" class=".btn">#4168</a>
            </td>
            <td>
                <b>
                    Change expiration for JWT authentification of engine port to 60 seconds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

The engine specification has changed the expiration time of JWT tokens. Before it as 5 seconds, now it is 60 seconds. This PR reflects this change in the spec.

https://github.com/ethereum/execution-apis/pull/256

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 12:28:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4166" class=".btn">#4166</a>
            </td>
            <td>
                <b>
                    Apply RocksDB LZ4 compression and compare post-sync metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Apply RocksDB LZ4 compression and compare the performance/resource metrics after sync.

Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 09:57:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4165" class=".btn">#4165</a>
            </td>
            <td>
                <b>
                    Fix dco on main branch build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

## PR description
Separate dco from spotless, make dco only run for pull requests.
Run on workflow dispatch on demand

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 04:08:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4164" class=".btn">#4164</a>
            </td>
            <td>
                <b>
                    Fix logIndex offset bug
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

The ethereum json-rpc spec requires `logIndex` be a log's position within the block:
https://ethereum.org/en/developers/docs/apis/json-rpc/#eth_getfilterchanges

This is also what's described in the comments, but instead the current implementation of logIndex starts counting only from the beginning of the current transaction.  This PR brings public transaction logs into conformance with the spec.

This does not include full support for changing logIndex to work the same way with private transactions, because this appears to require a change to the private state storage format.   Partial support has been included for review, but commented out due to non-existent privateStateStorage.getTransactionReceipts(blockHash) method.

Maybe it's not possible to access other private tx's in the same block?

TODO:  modify expected results for more tests, so that everything passes.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #4114 



## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 06:16:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4162" class=".btn">#4162</a>
            </td>
            <td>
                <b>
                    GitHub CI
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
Experiment moving the build to Github.

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-23 06:12:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4161" class=".btn">#4161</a>
            </td>
            <td>
                <b>
                    move some easy build jobs (DCO, Spotless) over to github
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>


## PR description
Move some of the work done by CircleCI to github actions

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 23:53:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4160" class=".btn">#4160</a>
            </td>
            <td>
                <b>
                    add goerli ttd
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
Add goerli TTD

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4159
## Documentation
![image](https://user-images.githubusercontent.com/1238512/180582277-a928edad-a18a-441e-ace3-c81e7f27ae21.png)

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 22:53:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4158" class=".btn">#4158</a>
            </td>
            <td>
                <b>
                    add sepolia mergeNetSplit block
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
Add sepolia fork next, aka mergeNetSplitBlock.  see https://github.com/ethereum/execution-specs/pull/564

Also:
* remove terminalBlockNumber from the list of forks (it is informational only)
* remove paris from list of forkblocks / aliases

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4157 

## Documentation
![image](https://user-images.githubusercontent.com/1238512/180582321-d4d89a5c-c59c-4c15-9abd-2563e687e574.png)

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 22:39:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4156" class=".btn">#4156</a>
            </td>
            <td>
                <b>
                    limit engine-api info logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Limit the info logging of the engine API:
* restrict fcU to one forkchoice log line to a max of once per minute
* drop logging of newPayload to debug 
* change invalid newPayload response to warn rather than info, and restrict this to a max of once per minute

Rather than not emitting useful information (like head, safe, and finalized block hashes), restrict the logging of this info so that periods of heavy traffic (like CL syncing) does not cause a torrent of log info

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4143 

## Documentation
![image](https://user-images.githubusercontent.com/1238512/180582361-f5b79dfa-3cf2-498f-9125-a0bcc69d5dd4.png)

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 20:41:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4155" class=".btn">#4155</a>
            </td>
            <td>
                <b>
                    Filter out the periodic log message "Refreshing DNS records with ..."
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

Filters out the log message `Refreshing DNS records with...` which is printed once per minute, to reduce the noise in the logs

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 20:37:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4150" class=".btn">#4150</a>
            </td>
            <td>
                <b>
                    fix 1 byte long disconnect reason
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Fixing https://github.com/hyperledger/besu/issues/4071

Signed-off-by: Stefan <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 09:18:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4149" class=".btn">#4149</a>
            </td>
            <td>
                <b>
                    Reduce RocksDB space amplification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reduce RocksDB space amplification with level_compaction_dynamic_level_bytes option set to true. In this case, the size target of levels is changed dynamically based on the size of the last level.

Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 15:27:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4148" class=".btn">#4148</a>
            </td>
            <td>
                <b>
                    add enr peers to discovery layer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
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
        Created At 2022-07-21 11:52:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4146" class=".btn">#4146</a>
            </td>
            <td>
                <b>
                    API Method: rollup_createPayload
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
Adds a new api method `rollup_createPayloadV1` as an extension to [Engine API](https://github.com/ethereum/execution-apis/blob/main/src/engine/specification.md) in order to allow to use Besu a L2 execution engine for Rollups;

This method allows to create a Payload with a given list of transactions, executed by it's given order. Invalid transactions are returned with error reason. Unprocessed transactions that don't fit within block gasLimit are returned as well.

To enable this method and rollup behaviour, Besu should run with `--engine-rollup-extension-enabled=true` on CLI

#### Request
Arguments:
- `parentBlockHash`: DATA, 32 Bytes - hash of parent block of this new payload;
- `transactions`:  Array of DATA - Array of transaction objects, each object is a byte list (DATA) representing TransactionType || TransactionPayload or LegacyTransaction as defined in [EIP-2718](https://eips.ethereum.org/EIPS/eip-2718)
- `prevRandao`: DATA, 32 Bytes - value for the prevRandao field of the new payload
- `feeRecipient`: DATA, 20 Bytes - suggested value for the feeRecipient field of the new payload
- `timestamp`: QUANTITY, 64 Bits - value for the timestamp field of the new payload

```json
{
    "id": "100",
    "jsonrpc": "2.0",
    "method": "rollup_createPayloadV1",
    "params": [
        "0xa326af38b7ad1ba192c00b89675c450ffd8e30d83c128ef37a62da26b9f58b9d",
        [
            "0xf86180820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8026a0b7b0cc34f06e99da2a0eb3f290be06fa5982e5b7883b9d2a46e09ee03861955ba008972a7505395050eb78e332d811049c824534a46d751b8305e1b3f819533017",
            "0xf8610a820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8025a09f0f2f41a2a7228d342b81f3937441a0767e5d78c25c86a8e5e5bec7e5fd3b33a02775ee8f94d673774f7f6fd090fa4ccd15b797a47236d59c0ad83549191660e4",
            "0xf86a01820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f96890ad78ebc5ac62000008025a0f6aee06079ff380ec5f0ef90f291b10450636698e9a8bf00484cb06d33713eaba01432b9e6739dcd50d4fbb0555be8a10c7aefb77364816b4493acbc608022deaf",
            "0xf86301820bb88405f5e10094f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8025a072d6b19aba780fdeb57fab5302bf142c5216f45c845267dca77f9d3e20910d44a05390bc4260c188e55a571f1d6a06ff9168391d4c8a7a498a2db49e41063f4b77",
            "0xf86101820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960c8026a096f3751f75a5eeb8f2e27167619ae24efcbb26cf1f5ee6d501ace868398c27dca0740ebd0912eae820d99083c671cf6a483b229a06e28d5e7a215b617cad24f28f",
            "0xf86180820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8026a0b7b0cc34f06e99da2a0eb3f290be06fa5982e5b7883b9d2a46e09ee03861955ba008972a7505395050eb78e332d811049c824534a46d751b8305e1b3f819533017"
        ],
        "0x284ae7412fa90216034852e4ecf953e69df541d323eb8c826442d7b71e5727f6",
        "0xcefc6c8fde4967c755e0e10144914e6d5571b088",
        "0x62d92263"
    ]
}
```

#### Response
```json
{
  "jsonrpc" : "2.0",
  "id" : "100",
  "result" : {
    "status" : "PROCESSED",
    "payloadId" : "0x000000002c94e08a",
    "executionPayload" : {
      "parentHash" : "0xa326af38b7ad1ba192c00b89675c450ffd8e30d83c128ef37a62da26b9f58b9d",
      "feeRecipient" : "0xcefc6c8fde4967c755e0e10144914e6d5571b088",
      "stateRoot" : "0xbce737f398b50b7675f36498184deff0ed134097890fc1ed8ebc2126d49a5ef5",
      "receiptsRoot" : "0xd95b673818fa493deec414e01e610d97ee287c9421c8eff4102b1647c1a184e4",
      "logsBloom" : "0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000",
      "prevRandao" : "0x284ae7412fa90216034852e4ecf953e69df541d323eb8c826442d7b71e5727f6",
      "blockNumber" : "0x1",
      "gasLimit" : "0x1c9c380",
      "gasUsed" : "0xa410",
      "timestamp" : "0x62d92263",
      "extraData" : "0x",
      "baseFeePerGas" : "0x7",
      "blockHash" : "0x13b7dab1660352dad22bcbb7462d03baf3aec68e5cc51bf599daccb21a2b79f7",
      "transactions" : [ "0xf86180820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8026a0b7b0cc34f06e99da2a0eb3f290be06fa5982e5b7883b9d2a46e09ee03861955ba008972a7505395050eb78e332d811049c824534a46d751b8305e1b3f819533017", "0xf86101820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960c8026a096f3751f75a5eeb8f2e27167619ae24efcbb26cf1f5ee6d501ace868398c27dca0740ebd0912eae820d99083c671cf6a483b229a06e28d5e7a215b617cad24f28f" ]
    },
    "unprocessedTransactions" : [ "0xf86301820bb88405f5e10094f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8025a072d6b19aba780fdeb57fab5302bf142c5216f45c845267dca77f9d3e20910d44a05390bc4260c188e55a571f1d6a06ff9168391d4c8a7a498a2db49e41063f4b77" ],
    "invalidTransactions" : [ {
      "transaction" : "0xf8610a820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8025a09f0f2f41a2a7228d342b81f3937441a0767e5d78c25c86a8e5e5bec7e5fd3b33a02775ee8f94d673774f7f6fd090fa4ccd15b797a47236d59c0ad83549191660e4",
      "reason" : "INCORRECT_NONCE",
      "errorMessage" : "transaction nonce 10 does not match sender account nonce 1."
    }, {
      "transaction" : "0xf86a01820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f96890ad78ebc5ac62000008025a0f6aee06079ff380ec5f0ef90f291b10450636698e9a8bf00484cb06d33713eaba01432b9e6739dcd50d4fbb0555be8a10c7aefb77364816b4493acbc608022deaf",
      "reason" : "UPFRONT_COST_EXCEEDS_BALANCE",
      "errorMessage" : "transaction up-front cost 0x00000000000000000000000000000000000000000000000ad78ebc5aca3cdb40 exceeds transaction sender account balance 0x00000000000000000000000000000000000000000000000ad78ebc5ac25eb236"
    } ]
  }
}
```


## Fixed Issue(s)
- #3760

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 10:09:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4145" class=".btn">#4145</a>
            </td>
            <td>
                <b>
                    logging changes for peering
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Signed-off-by: Stefan <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 07:20:25 +0000 UTC
    </div>
</div>

