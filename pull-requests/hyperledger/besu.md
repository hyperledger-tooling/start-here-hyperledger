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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2655" class=".btn">#2655</a>
            </td>
            <td>
                <b>
                    qbft block to transaction based voting migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Frame <jasonwframe@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Adds a migration so the existing qbft chains can move from block header based validation selection to using a smart contract for the validator selection.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 05:27:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2654" class=".btn">#2654</a>
            </td>
            <td>
                <b>
                    Refactor PKI ATs to only run subset of tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Using a new parameterized base class so PKI ATs to only run subset of tests

## Fixed Issue(s)
Fixes #2650 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 04:16:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2646" class=".btn">#2646</a>
            </td>
            <td>
                <b>
                    Add a labelled gauge to metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The labelled gauge functionality will allow monitoring of gauge type data without creating many gauges, which can be particularly handy in tracking related data.

This would be particularly useful in a specific use case in Teku which uses the besu infrastructure to provide prometheus metrics.
https://github.com/ConsenSys/teku/issues/3892

There are a large number of gauges that are requested, but logically they're actually a single gauge with labels capturing context.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 02:04:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2645" class=".btn">#2645</a>
            </td>
            <td>
                <b>
                    Refactor QbftExtraDataCodec from new instance to injection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Updated `RoundChange` and `ProposalPayload` `decode()` methods to accept a `BftExtraDataCodec` implementation (instead of creating a new instance of `QbftExtraDataCodec`.
- A bit of plumbing work all the way to `QbftBesuControllerBuilder`, where we choose the concrete codec instance to use.
- For the tests, we are using the `QbftExtraDataCodec` (to keep the previous behaviour)

fixes #2648

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 11:10:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2644" class=".btn">#2644</a>
            </td>
            <td>
                <b>
                    refactor GoQuorum private transaction detection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Refactor the GoQorum private transaction detection logic to be more DRY.

This also unifies `Transaction.isGoQuorumPrivateTransaction()` to also consider the `GoQuorumOptions.goQuorumCompatibilityMode` flag. Previously this flag was only considered in `TransactionDecoder`. This difference in behaviour could result in transaction encoding not being the inverse of transaction decoding.

## Fixed Issue(s)
fixes #2610

## Changelog
- [x] I thought about the changelog and ~~included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).~~ did not include a changelog update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 22:56:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2641" class=".btn">#2641</a>
            </td>
            <td>
                <b>
                    AcceptanceTests: Confirm transaction has been mined
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                AcceptanceTests: Confirm transaction has been mined before checking against privCall

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 08:41:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2640" class=".btn">#2640</a>
            </td>
            <td>
                <b>
                    Injecting BftExtraDataCodec into SubsequentMessageValidator
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
        Created At 2021-08-16 08:01:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2636" class=".btn">#2636</a>
            </td>
            <td>
                <b>
                    EIP-3074
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

## PR description
This adds the auth and authcall opcodes of EIP-3074 to Besu, as well as the Puxi testnet definition.

The PR is not ready for merge. It needs thorough review.

See #2637

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-14 18:03:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2635" class=".btn">#2635</a>
            </td>
            <td>
                <b>
                    Refactoring CmsValidator (internal CRL resolution)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span>
            </td>
            <td>
                ## PR description

Loading CRL list inside CmsValidator (instead of externally)

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-14 12:04:51 +0000 UTC
    </div>
</div>

