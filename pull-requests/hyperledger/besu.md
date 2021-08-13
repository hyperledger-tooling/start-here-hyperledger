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
                PR <a href="https://github.com/hyperledger/besu/pull/2631" class=".btn">#2631</a>
            </td>
            <td>
                <b>
                    Updating besu-native dependencies to 0.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

- Updating besu-native dependencies to 0.4.0
- Adding secp256r1 native lib

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 03:02:56 +0000 UTC
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
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
SECP256R1 is an an alternative signature algorithm which Besu supports. Until now there was only a Java implementation available. This PR adds a native library implementation for it. The native library will be used as default, following the SECP256K1 signature algorithm.

_Only this draft PR uses a snapshot version for testing, this will be replaced with a release version._ 

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2624" class=".btn">#2624</a>
            </td>
            <td>
                <b>
                    Feature/1559 cleanup tx price calc
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
* roll TransactionPriceCalculator into FeeMarket
* create a LegacyFeeMarket to use prior to London
* remove explicit usages of TransactionPriceCalculator static constructors
* remove TransactionPriceCalculator from ProtocolSpec (added to FeeMarket)
* make FeeMarket non-optional in ProtocolSchedule
* create BaseFeeMarket interface for London

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2559

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 00:12:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2622" class=".btn">#2622</a>
            </td>
            <td>
                <b>
                    Add Antony Denyer as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Antony has made [significant commits](https://github.com/hyperledger/besu/commits?author=antonydenyer) improving the quality and features of besu, this PR adds him as a maintainer.

Voting ends 2 weeks from the publication of this PR or once a majority of the maintainers [vote](https://github.com/hyperledger/besu/blob/master/MAINTAINERS.md#maintainers-approval-process).

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 09:10:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2621" class=".btn">#2621</a>
            </td>
            <td>
                <b>
                    Added PKI QBFT Block Creation Behaviour
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Refactored QbftRound, introducing the `CreateBlockForProposalBehaviour` Functional Interface.
  -  The default implementation uses the `BlockCreator`
  - The PKI implementation has the logic to add the CMS message into the proposed block' extra data
- Added PKI Logic into `ProposalPayloadValidator` 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 03:55:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2619" class=".btn">#2619</a>
            </td>
            <td>
                <b>
                    PKI Block Creation cli configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- added all CLI options for PKI Block Creation as a Mixin
- created `PkiBlockCreationConfigurationProvider` that will be used to inject the PkiOptions into QBFT-related objects

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-08 20:28:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2618" class=".btn">#2618</a>
            </td>
            <td>
                <b>
                    Permissioning - improve java docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Add some code snippets into java docs for permissioning plugin implementation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 09:39:21 +0000 UTC
    </div>
</div>

