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
                PR <a href="https://github.com/hyperledger/besu/pull/4024" class=".btn">#4024</a>
            </td>
            <td>
                <b>
                    Add Sepolia TTD and DNS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description

Adds the correct TTD and DNS config to the Sepolia config file

## Fixed Issue(s)
fixes #4021 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 09:06:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4023" class=".btn">#4023</a>
            </td>
            <td>
                <b>
                    Print full exception when NatService fails to configure automaticially
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/hyperledger/besu/issues/3787

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 08:56:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4019" class=".btn">#4019</a>
            </td>
            <td>
                <b>
                    allow upgrade whether websockets enabled or not
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>
fixes #3948 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 00:16:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4018" class=".btn">#4018</a>
            </td>
            <td>
                <b>
                    Updates to DNS discovery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Diego López León <dieguitoll@gmail.com>

## PR description
This PR adds a new implementation for [EIP-14159](https://eips.ethereum.org/EIPS/eip-1459) replacing [DNSDaemon](https://github.com/apache/incubator-tuweni/blob/main/dns-discovery/src/main/kotlin/org/apache/tuweni/discovery/DNSDaemon.kt) from Tuweni with a new one, vert.x based.
This new implementation provides the following benefits:
- Random tree traversal
- Batched discovery
- Periodic traversal continues from last state
- Non blocking implementation, based on vert.x DNS client 

## Fixed Issue(s)
Fixes #1707

## Notes
This is sent as a draft to gather feedback on this implementation. How often should we check the DNS for new peers? How many leaves should be attempted to connect per branch? Should this parameters need to be parameterized through the CLI? Based on the willingness to merge this proposal I would finish the specification by adding support to linked trees

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-27 19:33:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4017" class=".btn">#4017</a>
            </td>
            <td>
                <b>
                    warning invalid sync mode option [#3884]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Warning displayed to the user when an invalid sync-mode option passed to besu.
Removed the custom converter that was allowing invalid options to be passed converting them to null in the end.

## Fixed Issue(s)
Fixes #3884

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-27 01:16:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4013" class=".btn">#4013</a>
            </td>
            <td>
                <b>
                    Validate without saving2
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

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 15:02:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4011" class=".btn">#4011</a>
            </td>
            <td>
                <b>
                    Update reference tests to the latest version and include test for gray glacier
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">mainnet</span>
            </td>
            <td>
                The reference tests for Gray Glacier are included to ensure that our implementation is correct.

Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 11:45:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4010" class=".btn">#4010</a>
            </td>
            <td>
                <b>
                    typo minimum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

typo

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 05:34:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4009" class=".btn">#4009</a>
            </td>
            <td>
                <b>
                    Support dropping rocksdb column families
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

unsafe feature which allows dropping of column families.

Do not merge at present.

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
        Created At 2022-06-23 15:41:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4008" class=".btn">#4008</a>
            </td>
            <td>
                <b>
                    try updater protection
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
        Created At 2022-06-23 13:39:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4006" class=".btn">#4006</a>
            </td>
            <td>
                <b>
                    Improve logging in NatService
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Improve logging in NatService to clarify what's happening. Increase log severity as it can cause peers to fail to connect when running in k8s.

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 07:54:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4004" class=".btn">#4004</a>
            </td>
            <td>
                <b>
                    Version Upgrades for 22.7.0-RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update versions

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

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
        Created At 2022-06-23 02:04:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4003" class=".btn">#4003</a>
            </td>
            <td>
                <b>
                    Support free gas networks when using London fee market
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                In order to support [free gas private networks](https://besu.hyperledger.org/en/stable/HowTo/Configure/FreeGas/) in a London/EIP1559 context, I propose that we support setting a zero baseFee.

If `baseFeePerGas` is overridden as 0 wei, then bypass the need for a transaction to have a gas price of >= 7 wei.

The genesis would look something like this:
```
{
  "config": {
    ...
    "londonBlock": 0,
    ...
  },
  "baseFeePerGas": "0x0",
  "nonce": "0x0",
  ...
}
```

One potential downside is that once baseFeePerGas is set to 0, there's no going back for that chain. You can still use `--min-gas-price` to enforce _some_ gas, but the London base fee calculation will be forever opted out of as a consequence of the zero baseFee in the genesis block. This also means no ether would get burned since base fee will always be zero.

This is currently blocking users with free gas networks from upgrading past the Berlin fork.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Fixes https://github.com/hyperledger/besu/issues/3374
Fixes https://github.com/hyperledger/besu/issues/3763

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 00:41:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4002" class=".btn">#4002</a>
            </td>
            <td>
                <b>
                    [Issue 3867] Make eth subprotocol message size limit configurable
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
PR #2485 introduced a limit on incoming `eth` subprotocol message sizes.  However, there is no logic to force outgoing messages to conform to this size limit.  As a result of this asymmetry, a new node trying to sync with other besu nodes may end up disconnecting many of its peers for exceeding this limit.  This can cause nodes to get stuck during the sync process. 

This PR makes the max message size configurable via a hidden option: `--Xeth-max-message-size`.  This provides a workaround for nodes that are stuck in this way.  

Remaining TODOs (to be handled in follow-up PRs):
* Handle message size limit consistently by enforcing limits on outbound messages

## Fixed Issue(s)
This partially addresses the issue described in #3867. 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 22:10:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4001" class=".btn">#4001</a>
            </td>
            <td>
                <b>
                    EthPeers unique
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stefan <stefan.pingel@consensys.net>

## PR description

To fix some issues that have been reported this PR makes sure that in EthPeers only has one EthPeer for each individual peer. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 09:32:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4000" class=".btn">#4000</a>
            </td>
            <td>
                <b>
                    large executor for qats
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Seeing periodic failures on the Quorum ATs which can pass after re-running. Changing to large executor should help this.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 00:02:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3999" class=".btn">#3999</a>
            </td>
            <td>
                <b>
                    Backwards Sync now adding blocks to BadBlocksManager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes: #3942
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 14:41:09 +0000 UTC
    </div>
</div>

