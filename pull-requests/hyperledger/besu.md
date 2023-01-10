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
                PR <a href="https://github.com/hyperledger/besu/pull/4903" class=".btn">#4903</a>
            </td>
            <td>
                <b>
                    Preload node and not only rlp
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
        Created At 2023-01-10 14:28:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4902" class=".btn">#4902</a>
            </td>
            <td>
                <b>
                    [RPC] add SAFE and FINALIZED options for block param
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">RPC</span>
            </td>
            <td>
                RPC method changes
- add SAFE and FINALIZED options for block param
- check length of blockNumber / blockHash param - if it's too short to be a blockHash and too long to be a blockNumber, throw Invalid params
- added some extra tests. Specifically this file `eth_getTransactionCount_invalidBlockNumber.json` - without the code changes in this PR, that spec test returns "block not found", with these changes returns Invalid params

See #4233 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 05:02:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4900" class=".btn">#4900</a>
            </td>
            <td>
                <b>
                    Support Shanghai in Reference Tests
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

Add support for Shanghai in reference tests
* Add Shanghai and Cancun milestones
* Add "withdrawals" and "withdrawalsRoot" to json objects
* Migrate to schedule by block header.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

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
        Created At 2023-01-09 23:07:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4899" class=".btn">#4899</a>
            </td>
            <td>
                <b>
                    fix toml parsing of double type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix toml config file parsing for options that map to type Double. Previously setting a value in toml config for a long option type would result in, e.g. :

```
Value of 'tx-pool-limit-by-account-percentage' is a float
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 16:03:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4898" class=".btn">#4898</a>
            </td>
            <td>
                <b>
                    EOF Optimization - don't split code sections
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

Optimize the EOF Functions implementation by not splitting code sections into separate Bytes object.  Instead the EOF evaluation occurs on a single container space.  When a function is called the PC (relative to container start, not section start) is moved, and no section re-loading needs to occur.

EOF lacks PC introspection and absolute jumps, so where "PC=0" starts is not observable to the code.

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
        Created At 2023-01-09 15:44:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4897" class=".btn">#4897</a>
            </td>
            <td>
                <b>
                    use bonsai updater cache to avoid calling database several times for the same account
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …the same value

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
        Created At 2023-01-09 14:22:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4895" class=".btn">#4895</a>
            </td>
            <td>
                <b>
                    For TimestampSchedule (Shanghai) remove evmBuilder override but leave other mods in
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                Ideally, want to remove all the modifications, but that will be addressed by https://github.com/hyperledger/besu/issues/4788
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 08:12:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4893" class=".btn">#4893</a>
            </td>
            <td>
                <b>
                    Remove qbft reference tests
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
Removes the QBFT reference tests as these are only being used by Besu and these same tests are covered in the integration tests.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4187 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 05:14:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4892" class=".btn">#4892</a>
            </td>
            <td>
                <b>
                    Withdrawals type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add withdrawals type with rlp encoding and decoding

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 03:01:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4890" class=".btn">#4890</a>
            </td>
            <td>
                <b>
                    Implement engine_forkchoiceUpdated Withdrawals validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Spec: https://github.com/ethereum/execution-apis/blob/main/src/engine/shanghai.md

In order to avoid maintaining two versions of forkchoiceUpdated as much as possible, the validation works for both V1 and V2.

The JSON deserialization allows for withdrawals to be omitted which supports V1 requests, however if shanghai is enabled then we will expect withdrawals in a V1 request. I think it would be a bug for a CL to send V1 with null withdrawals if the payload attributes had a post-shanghai timestamp.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Part of #4776 

Follows on from https://github.com/hyperledger/besu/pull/4876
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-08 22:53:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4888" class=".btn">#4888</a>
            </td>
            <td>
                <b>
                    Peering - disconnect worst peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Disconnect "worst" peer in two cases
* AbstractRetryingSwitchingPeerTask - when retrying task with multiple peers and all peers have been tried and found wanting
* FastSyncTargetManager - if best peer is behind the pivot block, disconnect worst peer 
Also add some extra context info to "Best peer" log message

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 07:01:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4887" class=".btn">#4887</a>
            </td>
            <td>
                <b>
                    Update changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Zhenyang Shi <wcgcyx@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Move chain pruning feature to 23.1.0-beta and add notice to the feature.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 06:11:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4884" class=".btn">#4884</a>
            </td>
            <td>
                <b>
                    Move EOF to Cancun
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

Move the EOF changes from Shanghai into the Cancun fork.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

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
        Created At 2023-01-05 20:14:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4883" class=".btn">#4883</a>
            </td>
            <td>
                <b>
                    Calculate block value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Zhenyang Shi <wcgcyx@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR adds the block value calculation to engine_getPayloadV2. 

Block value is calculated as the sum of the block's priority fee as per the current [spec](https://github.com/ethereum/execution-apis/blob/main/src/engine/shanghai.md#specification-2). 

However, the calculated block value isn't strictly equal to the balance diff of the fee recipient as it doesn't capture balance gain through transaction execution (balance transfer, contract logic...). For example, tx1 may have less priority fee than tx2 but tx1 involves a direct transfer to fee recipient thus overall makes tx1 better than tx2.

Using the sum of the block's priority fee is the most straight-forward way to calculate the block value as a starting point as it only involves very minimum change. A future improvement is to have block processor report the balance diff of the fee recipient either during block creation or block validation and use that as the actual block value because re-evaluating the block value in get payload call will consume a lot of time. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4861 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 04:29:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4879" class=".btn">#4879</a>
            </td>
            <td>
                <b>
                    Deprecation warning for Goquorum privacy mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a warning if besu is started with isQuorum mode in genesis file. 
Advise to use `--privacy-enabled` instead

Fixes #4848 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 02:25:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4876" class=".btn">#4876</a>
            </td>
            <td>
                <b>
                    Create skeleton structure for Engine API V2 methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

First step to implementing https://github.com/ethereum/execution-apis/blob/main/src/engine/shanghai.md

Create AbstractEngineNewPayload and AbstractEngineForkchoiceUpdated, extending with V1 and V2 versions.
(AbstractEngineGetPayload and V2 was already introduced in https://github.com/hyperledger/besu/commit/a483f79cc8b7741cb9fb0145d92307b6d5cfdc62)

This will be the basis for parallelising getting a productionised version of the Withdrawals draft onto main. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Part of https://github.com/hyperledger/besu/issues/4776

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 23:27:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4875" class=".btn">#4875</a>
            </td>
            <td>
                <b>
                    Worldstate-only resync behavior
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
Implements a  debug rpc endpoint and a behavior to resync just the worldstate.  

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
        Created At 2023-01-03 21:57:11 +0000 UTC
    </div>
</div>

