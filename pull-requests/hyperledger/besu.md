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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2634" class=".btn">#2634</a>
            </td>
            <td>
                <b>
                    Jumpdest analysis
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

Adds ability to cache Code objects and use them for future calls which will avoid the re-computing of JUMP destinations. 
No additonal tests have been added to demonstrate performance improvement. The correct place for those remains an open question.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #2607 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 23:21:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2633" class=".btn">#2633</a>
            </td>
            <td>
                <b>
                    Fixed nonce bug in EthGetTransactionCount
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">testing</span>
            </td>
            <td>
                ## PR description

Fixed bug where EthGetTransactionCount would return a lower value for pending than latest when there are old transactions in the transaction pool.

Wrote a failing test to show the expected behaviour and ensured that the max of latest and pending is used.


## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 22:55:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2632" class=".btn">#2632</a>
            </td>
            <td>
                <b>
                    refactor of  GasLimitCalculator into protocolSchedule
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

this is an extensive re-plumbing to make GasLimitCalculator part of ProtocolSchedule rather than being global

highlights:
* plumbing of `Optional<AtomicLong>` targetGasLimit into MiningParameters, MiningCoordinators, MiningExecutors, and Block Creators
* moving GasLimitCalculator interface and related implementations into ethereum:core
* creation of LondonTargetingGasLimitCalculator
* removal of 1559 specific forkblock gas limit logic in GasLimitRangeAndDeltaValidationRule and AbstractBlockCreator

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2561 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 22:43:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2630" class=".btn">#2630</a>
            </td>
            <td>
                <b>
                    Add native secp256r1 lib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
SECP256R1 is an an alternative signature algorithm which Besu supports. Until now there was only a Java implementation available. This PR adds a native library implementation for it. The native library will be used as default, following the SECP256K1 signature algorithm.

~~Only this draft PR uses a snapshot version for testing, this will be replaced with a release version.~~

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 20:25:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2625" class=".btn">#2625</a>
            </td>
            <td>
                <b>
                    QBFT - Create extradata with round information only
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Create extra data with round information only when using a contract to obtain vote and validators information.
 
## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 07:53:26 +0000 UTC
    </div>
</div>

