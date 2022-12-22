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
                PR <a href="https://github.com/hyperledger/besu/pull/4859" class=".btn">#4859</a>
            </td>
            <td>
                <b>
                    EOF updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                EOF changes tracking Breakout room #4 changes.
Also, add more test coverage.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

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
        Created At 2022-12-22 08:07:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4858" class=".btn">#4858</a>
            </td>
            <td>
                <b>
                    Move EVM operation Tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Move the EVM individual operation tests into the EVM module.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 22:24:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4855" class=".btn">#4855</a>
            </td>
            <td>
                <b>
                    rollback dco on push
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <macfarla.github@gmail.com>

The action we're using here only supports pull_request events
https://github.com/tim-actions/get-pr-commits/blob/c64db31d359214d244884dd68f971a110b29ab83/index.js#L4

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 20:03:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4854" class=".btn">#4854</a>
            </td>
            <td>
                <b>
                    not save invalid trie log
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
        Created At 2022-12-21 16:13:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4853" class=".btn">#4853</a>
            </td>
            <td>
                <b>
                    'No sync target' logging improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">logging</span>
            </td>
            <td>
                Signed-off-by: mark-terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
"No sync target, checking current peers for usefulness" logging made less spammy, with improved detail.
- DEBUG level log message rate reduced to once every 15 seconds, with pivot block target added to logging message.
- INFO level log message added at 2 minute intervals to provide user feedback while import is paused

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Addresses #4794

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 03:43:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4847" class=".btn">#4847</a>
            </td>
            <td>
                <b>
                    DCO check on main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                fixes #4837

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 22:28:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4846" class=".btn">#4846</a>
            </td>
            <td>
                <b>
                    [Minor] Delete unused classes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Originally committed in https://github.com/hyperledger/besu/commit/435c9e388c160e30e39856c2eaea0147779a953a

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 20:55:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4845" class=".btn">#4845</a>
            </td>
            <td>
                <b>
                    EOF Code Validation CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description

A CLI tool to validate EOF formatted code.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 17:58:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4844" class=".btn">#4844</a>
            </td>
            <td>
                <b>
                    PoS checkpoint sync
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
Enables PoS checkpoint sync under an experimental flag

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #4573

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 14:23:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4843" class=".btn">#4843</a>
            </td>
            <td>
                <b>
                    Fix some flaky tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <macfarla.github@gmail.com>

- increase timeout for OpenTelemetry trace test
- override port conflict check in BesuCommandTest

fixes #4670 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 02:49:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4842" class=".btn">#4842</a>
            </td>
            <td>
                <b>
                    Ignore extra RocksDB column families for experimental features
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
This PR adds the support to ignore certain column family to support having experimental feature store data in rocksdb. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4831 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 01:53:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4841" class=".btn">#4841</a>
            </td>
            <td>
                <b>
                    EIP-6122 Timestamp based fork IDs
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
Timestamp based fork IDs implementing [EIP-6122](https://github.com/ethereum/EIPs/pull/6122)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 00:27:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4839" class=".btn">#4839</a>
            </td>
            <td>
                <b>
                    Deprecation notice for GoQuorum-compatible privacy and IBFT 1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <macfarla.github@gmail.com>

Besu currently has 3 privacy modes. The privacy mode that provides compatibility with GoQuorum privacy is intertwined with mainnet code at the transaction and block processing level. We also have not seen demand for this privacy mode within the Besu community.
We plan to deprecate the GoQuorum-compatible privacy feature, along with IBFT 1.0, in the coming quarterly release 23.1, and then remove it in the following quarterly release 23.4.
Removing the code associated with this feature will reduce the complexity of the transaction and block processing code, reducing friction for mainnet-focused development.

This will not affect the remaining 2 privacy modes (EEA privacy and flexible privacy groups).
This will not affect IBFT 2.0 or QBFT.

Reach out to us on Discord with any questions.

Also remove quorum ATs nightly task - this nightly task is currently consistently failing. Since we are deprecating the GoQuorum-compatible privacy feature in 23.1 so we won't be investing time fixing these tests.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 11:05:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4836" class=".btn">#4836</a>
            </td>
            <td>
                <b>
                    Optimize Sstore operation execution time
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR aims to improve SStore operation execution time by getting the original value and current value only once during gas cost and refund calculation. Currently, we make these two calls twice, and even with RocksDB cache, this has an impact on SStore performance as we can see in the CPU profiling flame graph below.
<img width="1187" alt="image" src="https://user-images.githubusercontent.com/5099602/208313044-7abc0ea3-1f39-4fe4-aaf8-87cec2b3e3e8.png">


After this PR, we can see that getSorageValue (get current value) and getOriginalStorageValue are called only once.
<img width="1720" alt="image" src="https://user-images.githubusercontent.com/5099602/208313255-54a9a9c2-d362-495a-b6b5-60efe4a43a38.png">

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
        Created At 2022-12-18 14:06:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4834" class=".btn">#4834</a>
            </td>
            <td>
                <b>
                    Fix javadocs to allow doc lint to pass in JDK 16 and above.
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
Adding missing javadocs so that javadoc doclint passes against JDK 16+ (invoke by Besu gradle build).

Exclude following packages from javadoc lint:
- org.hyperledger.besu.privacy.contracts.generated
- org.hyperledger.besu.tests.acceptance.*

Temporarily exclude ethereum and evm submodule for doc lint checks.

Fixed Issue(s)
https://github.com/hyperledger/besu/issues/2681

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 07:01:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4833" class=".btn">#4833</a>
            </td>
            <td>
                <b>
                    Initial implementation of EngineGetPayloadV2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span><span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Gabriel Trintinalia <gabriel.trintinalia@gmail.com>


## PR description
Initial implementation of EngineGetPayloadV2

- Same result as V1 but adds the block value to the payload:
- Calculate Block Value currently does not have an implementation and will return 0

```
{
    "jsonrpc": "2.0",
    "id": 67,
    "result": {
        "executionPayload": {
            "parentHash": "0x3b8fb240d288781d4aac94d3fd16809ee413bc99294a085798a589dae51ddd4a",
            "feeRecipient": "0xaa00000000000000000000000000000000000000",
            "stateRoot": "0xca3149fa9e37db08d1cd49c9061db1002ef1cd58db2210f2115c8c989b2bdf45",
            "logsBloom": "0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000",
            "prevRandao": "0xff00000000000000000000000000000000000000000000000000000000000000",
            "gasLimit": "0x1c9c380",
            "gasUsed": "0x0",
            "timestamp": "0x50",
            "extraData": "0x",
            "baseFeePerGas": "0x7",
            "transactions": [],
            "blockNumber": "0x1",
            "blockHash": "0xae199cf83e812e4eb14e9597ce82b743c01e494c6fe660eab144b0a97e9fdb4d",
            "receiptsRoot": "0x56e81f171bcc55a6ff8345e692c0f86e5b48e01b996cadc001622fb5e363b421"
        },
        "blockValue": "0x0"
    }
}

```

## Fixed Issue(s)
See https://github.com/ethereum/execution-apis/issues/307

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 05:21:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4832" class=".btn">#4832</a>
            </td>
            <td>
                <b>
                    Use blocking executor in test
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
Switch to blocking executor in chain pruner test so pruning happened in the same thread.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4830 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 02:22:33 +0000 UTC
    </div>
</div>

