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
                PR <a href="https://github.com/hyperledger/besu/pull/2686" class=".btn">#2686</a>
            </td>
            <td>
                <b>
                    typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Fix 2 typos.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-28 04:19:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2685" class=".btn">#2685</a>
            </td>
            <td>
                <b>
                    Eth66 protocol should only apply to the Eth protocol
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
Besu using the instanbul/99 or instanbul/100 incorrectly encodes messages with a requestId from eth66.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #2682

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 07:47:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2684" class=".btn">#2684</a>
            </td>
            <td>
                <b>
                    address clique london HeaderValidator config
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

address clique BlockHeaderValidator configuration issue for london fee market

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2680 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 06:57:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2683" class=".btn">#2683</a>
            </td>
            <td>
                <b>
                    Use native SECP256K1 and SECP256R1 for signature normalization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use native SECP256K1 for signature normalization

Add support for SECP256K1 "normalize" path to use the native library.

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 02:22:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2677" class=".btn">#2677</a>
            </td>
            <td>
                <b>
                    Adding QBFT PKI-backed Block Creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                ## PR description
- Changed `cms` field in `PkiExtraData` from `Optional<Bytes>` to `Bytes`
- Updated PkiExtraData encoding/decoding. Now we are appending the CMS as the last element in the ExtraData list.
- Created `QbftContext` containing the optional `PkiBlockCreationConfiguration`. Used to determine if the node is running in PKI mode and to have access to the KeyStores.
- Created a new hashing strategy that excludes the CMS data from the hash calculation. This is used when calculating the signed hash inside the CMS message.
- Updated `QbftRound` with a new `createBlockForProposalBehaviour`. The default implementation just creates the block. The "PKI" implementation created the block and adds the CMS into the extra data.
- Updated `ProposalPayloadValidator` with logic to validate the CMS message in the proposal (when running in PKI-mode).
- Included `pki-qbft` parameter for PKI ATs. This will run tests using PKI QBFT.

## Pending Changes
- [x] Stop leaking PKI information to `BftExtraDataCodec` (we are leaking it through the `EXCLUDE_CMS` enum value)
- [ ] Remove duplication on `PkiQbftExtraDataCodec#encode(..)` method (we are duplicating code from `QbftExtraDataCodec#encode`)

## Fixed Issue(s)
fixes #2653 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-26 01:04:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2676" class=".btn">#2676</a>
            </td>
            <td>
                <b>
                    implement EIP-3607
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

implement [EIP-3607: Reject transactions from senders with deployed code](https://eips.ethereum.org/EIPS/eip-3607)

The [expectation in ACD](https://discord.com/channels/595666850260713488/745077610685661265/877128936813891634) is that this attack is not possible currently, so there should not be any need to gate this behavior on protocol schedule, since it should never have happened.
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2663 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 19:43:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2675" class=".btn">#2675</a>
            </td>
            <td>
                <b>
                    A plugin implementer may register the payload provider in start or register
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

When registering a PrivacyPluginService you need to call setPayloadProvider before blocks get mined. You have two opportunities to do this, once when besu calls register in your plugin and once when besu calls start in your plugin.

Ideally, you would setPayloadProvider when register is called. That way Besu can confirm that you've set the various command line options correctly in BesuCommand. But the problem is when Besu calls register it hasn't yet parsed the command line args into. So if you've got some cli arguments set in your plugin they will not be populated yet.


## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 14:44:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2674" class=".btn">#2674</a>
            </td>
            <td>
                <b>
                    DRY onchain management proxies
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

Read-only access to the on-chain privacy group contract is centralized to happen in `OnchainPrivacyGroupContract` only. 

## Fixed Issue(s)
fixes #1303
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 09:16:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2673" class=".btn">#2673</a>
            </td>
            <td>
                <b>
                    Update memory to use MutableBytes
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

This modification improves performance because we no longer have to copy the memory to a new array every time we want to read it.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 08:35:35 +0000 UTC
    </div>
</div>

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

