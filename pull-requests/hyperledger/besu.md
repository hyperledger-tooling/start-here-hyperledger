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
                PR <a href="https://github.com/hyperledger/besu/pull/2557" class=".btn">#2557</a>
            </td>
            <td>
                <b>
                    Privacy plugin pmt factory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

Allow a plugin to sign private marker transactions. When registering the `PrivacyPluginService` setting the `PrivateMarkerTransactionFactory` is optional and will fall back to either fixed or random if not specified.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 07:19:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2549" class=".btn">#2549</a>
            </td>
            <td>
                <b>
                    Switch to dynamic version calculation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

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
        Created At 2021-07-20 14:15:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2547" class=".btn">#2547</a>
            </td>
            <td>
                <b>
                    Privacy plugin pmt signer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Allow plugin users to sign privacy marker transactions
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 12:37:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2545" class=".btn">#2545</a>
            </td>
            <td>
                <b>
                    Tx replacement rules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
refactor of transaction replacement rules:
* split into gasPrice and 1559FeeMarket rules
* consider maxFeePerGas as well as maxPriorityFeePerGas in the transaction bump logic for 1559 fee market

1559 fee market logic is effectively:
* replace when BOTH:
  * new effective price  > prior effective price plus percent bump 
  * new effective priority fee is >= prior effective priority fee
* OR, replace when BOTH:
  * new effective price == prior effective price 
  * new effective priority fee > prior effective priority fee plus percent bump
* ELSE, don't replace



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
fixes #2529

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 22:43:40 +0000 UTC
    </div>
</div>

