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
                PR <a href="https://github.com/hyperledger/besu/pull/3788" class=".btn">#3788</a>
            </td>
            <td>
                <b>
                    [MINOR] fixed some errors from CodeQL
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * dereferenced variable is always null in log message

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 23:04:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3784" class=".btn">#3784</a>
            </td>
            <td>
                <b>
                    Preparing for next version and 22.4.0 Changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

- Preparing for next release
- 22.4.0 changelog
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 05:13:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3783" class=".btn">#3783</a>
            </td>
            <td>
                <b>
                    Release 22.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Release 22.4.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 05:06:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3782" class=".btn">#3782</a>
            </td>
            <td>
                <b>
                    [MINOR] Typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixed typos

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 00:28:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3780" class=".btn">#3780</a>
            </td>
            <td>
                <b>
                    [MINOR] code cleanup - Lists.emptyList
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - changed some Longs to long where they were statically intialized
- changed random.nextLong() to random.nextInt(Integer.MAX_VALUE) to avoid the edge case of long minimum value which gives a negative value when passed into abs()
- replace deprecated Lists.emptyList() with Collections.emptyList()

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-03 11:58:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3778" class=".btn">#3778</a>
            </td>
            <td>
                <b>
                    [DO NOT MERGE] Performance test : test Amazon ACCP
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
Test Amazon ACCP implementation
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
        Created At 2022-04-29 09:43:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3777" class=".btn">#3777</a>
            </td>
            <td>
                <b>
                    changed for loops with int vs long comparison
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Where int was being compared with long. Mostly int being used to iterate over values which could be long.
Not sure about these 2 since they are dealing with uint
- FlexiblePrivacyGroupContract
- FlexiblePrivacyGroupController

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 06:43:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3776" class=".btn">#3776</a>
            </td>
            <td>
                <b>
                    Remove Leading Zeros from TransactionPendingResult
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                ## PR description

Currently, there is an issue with the way `TransactionPendingResult` gets serialized by in the JSON-RPC subsystem. Specifically, when responding to `eth_getTransactionByHash,` the `gasPrice`, `maxFeePerGas`, and `maxPriorityFeePerGas` values should be Quantities without leading zeros like so:

```
    "gas" : "0x11e63",
    "gasPrice" : "0x77359407",
    "maxPriorityFeePerGas" : "0x77359400",
    "maxFeePerGas" : "0xd09dc3000",
```

This is the official behavior defined in the spec and the behavior demonstrated by Geth and Nethermind.

However, in Besu, they are treated like 32-byte arrays and serialized with the leading zeros in place:

```
    "gas" : "0x10c83",
    "gasPrice" : "0x0000000000000000000000000000000000000000000000000000000ab5d04c00",
    "maxFeePerGas" : "0x0000000000000000000000000000000000000000000000000000000ab5d04c00",
```

This is a simple oversight caused by using `Wei.toHexString()` instead of `Wei.toShortHexString()`, which this PR addresses.

@frankisawesome has offered to fix the relevant unit tests that were unable to catch this, and will attach the fixes to this PR when they are ready.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 05:24:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3774" class=".btn">#3774</a>
            </td>
            <td>
                <b>
                    adding codeql to besu to check for quality
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
Adding codeql scans to HLF Besu


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 05:21:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3773" class=".btn">#3773</a>
            </td>
            <td>
                <b>
                    fix nullpointer on snapsync
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

Fixes a bug that caused Besu to not restart healing properly when changing pivot blocks. Snapsync thought the sync was done instead of restarting on a new pivot block. 

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
        Created At 2022-04-28 15:11:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3772" class=".btn">#3772</a>
            </td>
            <td>
                <b>
                    update version and changelog
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
        Created At 2022-04-28 09:56:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3771" class=".btn">#3771</a>
            </td>
            <td>
                <b>
                    update version to 22.4.0-RC3-SNAPSHOT
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
        Created At 2022-04-28 09:34:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3770" class=".btn">#3770</a>
            </td>
            <td>
                <b>
                    Release 22.4.0-RC2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release 22.4.0-RC2
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 08:57:24 +0000 UTC
    </div>
</div>

