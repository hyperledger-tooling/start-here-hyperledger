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
                PR <a href="https://github.com/hyperledger/besu/pull/2578" class=".btn">#2578</a>
            </td>
            <td>
                <b>
                    Updated CHANGELOG
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Updating CHANGELOG with missing features.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 21:34:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2577" class=".btn">#2577</a>
            </td>
            <td>
                <b>
                    EIP1559 Cleanup : remove experimental flags 
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

We need to clean the ExperimentalEIPs class by removing this flags

This was configurable when developing the EIP now the values have been defined in the spec and cannot change via a flags without creating a consensus bug issue on the mainnet

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 12:39:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2576" class=".btn">#2576</a>
            </td>
            <td>
                <b>
                    Add support for mining ommers, up to 8 blocks behind the head job
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
This allows miners to send solutions for blocks up to 8 blocks behind head, to be included as ommers.

## Fixed Issue(s)
Fixes #2572

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-25 18:04:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2575" class=".btn">#2575</a>
            </td>
            <td>
                <b>
                    2496 ping pong encoding error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->
There are clients that send PING messages without a from field. The devp2p spec doesn't indicate that these are optional, but we will try to handle them as if they were.

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #2496 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 20:04:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2574" class=".btn">#2574</a>
            </td>
            <td>
                <b>
                    Qbft to use validator contract
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
Qbft to use validator contract

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 04:55:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2573" class=".btn">#2573</a>
            </td>
            <td>
                <b>
                    Added abstract BftBesuControllerBuilder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Introduced an abstract `BftBesuControllerBuilder` with supplier methods that enable concrete implementations to provide the desired concrete `ExtraDataCodec` and `BftBlockInterface`.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 23:01:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2570" class=".btn">#2570</a>
            </td>
            <td>
                <b>
                    Bft validator provider
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
QBFT uses the same validator management logic that IBFT2 and IBFT use and allows for a lot of code reuse. This will make it possible for bft based consensus mechanism to use it's own specific mechanism to manage validators i.e. determining what the validators are and the mechanism to add and remove them.

This is needed so that QBFT can move using transaction based validator management using smart contracts.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 04:50:14 +0000 UTC
    </div>
</div>

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

The interface has changed to 

```
public interface PrivateMarkerTransactionFactory {
  Address getSender(PrivateTransaction privateTransaction, String privacyUserId);

  Bytes create(
      UnsignedPrivateMarkerTransaction unsignedPrivateMarkerTransaction,
      PrivateTransaction privateTransaction,
      String privacyUserId);
}

```

The factory is responsible for RLP encoding and signing. It should have all the information it needs to make a decision about how to sign the marker transaction. Nothing else should be required before submitting to the transaction pool.

The `getSender` method is used to help facilitate a stripped locking strategy for nonce calculation. When the create method is called you can be assured that it will not be called again for that address until it has finished submitting it to the transaction pool. 

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

