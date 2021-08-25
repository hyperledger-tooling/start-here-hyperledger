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
                PR <a href="https://github.com/hyperledger/besu/pull/2670" class=".btn">#2670</a>
            </td>
            <td>
                <b>
                    Updated ATs DSL to create PKI QBFT node configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Exposing utility classes from `:pki` module
- Simplified `PkiKeyStoreConfiguration` replacing password **supplier** with actual password file path
- Added `createPkiQbftNode` method on BesuNodeFactory
- Updated Thread and Process runner to consume PKI configuration when starting nodes
- Created `PkiKeystoreConfigurationFactory` responsible for creating PKI config (including certificate temp files and issuing certs from the same CA).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 04:15:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2669" class=".btn">#2669</a>
            </td>
            <td>
                <b>
                    Updated besu-native to 0.4.2 for ec libraries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

- Updated besu-native to 0.4.2 for ec libraries
- Not updating bls12-381 because of https://github.com/hyperledger/besu/issues/2668

## Fixed Issue(s)
fixes #2665

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 10:37:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2667" class=".btn">#2667</a>
            </td>
            <td>
                <b>
                    Updated permissioning controller to handle both DNS and IP rules.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mark Terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Updates the permissioning controller to handle rules with both IP and DNS entries.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #2571 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-21 13:21:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2666" class=".btn">#2666</a>
            </td>
            <td>
                <b>
                    Upgrade to OpenTelemetry 1.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>


## PR description
Upgrade to latest OpenTelemetry release.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-21 06:50:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2664" class=".btn">#2664</a>
            </td>
            <td>
                <b>
                    Remove duplicate AddOperation on MainnetEvmRegistries
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
While familiarizing myself with the EVM code, I noticed that there is a duplicate `AddOperation` being added to the `MainnetEvmRegistries`. The `MainnetEvmRegistries#put()` function just assigns the operation to a map using the operation's opcode so removing this duplicate line has no effect on the EVM itself as it was just overwriting the previous line.

## Fixed Issue(s)


## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 23:53:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2661" class=".btn">#2661</a>
            </td>
            <td>
                <b>
                    Expose args in PicoCLIOptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Allow plugins to see what arguments were used to start besu.

Form inside a plugin I need to be able to get access to arguments that were used to start besu, specifically 

`--rpc-http-port`
`--rpc-http-enabled`
`--rpc-http-tls-enabled`


## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 09:26:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2660" class=".btn">#2660</a>
            </td>
            <td>
                <b>
                    Encapsulate London Block transaction gas price validation
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
* add BaseFeeBlockBodyValidator extends MainnetBlockBodyValidator
* use in London protocolschedule
 
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2565

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 22:13:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2659" class=".btn">#2659</a>
            </td>
            <td>
                <b>
                    Split Transaction Gas Calculation from EVM Calculation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In preparation for the EVM library pull out the transaction related gas
calculations and move them into their own `TransactionGasCalculator.`

This has 4 calls right now, none of which occur inside the EVM:
* Intrinsic gas cost
* Code Deposit gas cost
* Max refund quotient
* Max Privacy Marker Transaction intrinsic gas cost.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 23:41:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2658" class=".btn">#2658</a>
            </td>
            <td>
                <b>
                    Feature/1559 cleanup remove 1559 object
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
* absorb EIP1559 objects into BaseFeeMarket
* remove explicit EIP1559 plumbing and rely on ProtocolSchedule where possible


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #2562

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 23:17:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2657" class=".btn">#2657</a>
            </td>
            <td>
                <b>
                    Remove EIP-1702 account versioning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                EIP-1702 versioning was a candidate for the Istanbul hard fork but was
removed prior to the first testnet. Other versioning techniques have
greater core dev mind share and one preparatory step landed in London,
EIP-3541, making EIP-1702 very unlikely to make it to mainnet.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 16:32:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2656" class=".btn">#2656</a>
            </td>
            <td>
                <b>
                    Update pending transaction manager
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

This PR add different ways of sorting transactions in the pool regarding the fork present (whether or not the genesis has the london fork) .
- Back to simple sorting for pre-london blockchains (based on gasPrice)
- Setting up a more complex sorting for blockchains with the london fork (to manage eip1559 transactions)

This makes it possible to simplify the code by putting different sorting method according to what we need .



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2563 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 13:27:26 +0000 UTC
    </div>
</div>

