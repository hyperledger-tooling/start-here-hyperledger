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
                PR <a href="https://github.com/hyperledger/besu/pull/2347" class=".btn">#2347</a>
            </td>
            <td>
                <b>
                    update CHANGELOG for 21.1.7 release
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

update CHANGELOG for 21.1.7 release


## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 16:30:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2346" class=".btn">#2346</a>
            </td>
            <td>
                <b>
                    Prepare for version 21.1.8-SNAPSHOT
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
        Created At 2021-06-01 15:47:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2345" class=".btn">#2345</a>
            </td>
            <td>
                <b>
                    Release 21.1.7
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
        Created At 2021-06-01 15:28:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2343" class=".btn">#2343</a>
            </td>
            <td>
                <b>
                    Add calaveras testnet and remove baikal
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

Add calaveras testnet and remove baikal for London

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-31 12:17:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2342" class=".btn">#2342</a>
            </td>
            <td>
                <b>
                    Fix invalid upfrontgascost modification for EIP1559
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

Obviously the last 1559 modification made causes a consensus issue on Baikal while the 4 rules are valid
- The block http://18.224.51.102:3000/block/14498
- The modification https://github.com/hyperledger/besu/pull/2338/files#diff-8f3af0f8da1b352c31d41501c14cf92a66947bc3dc2a2f0d617c1691c380c70fR539
This change decrement the balance of the wallet here https://github.com/hyperledger/besu/blob/3267501c8cd2a1cd116b8b295e5baedab12bd3b5/[…]erledger/besu/ethereum/mainnet/MainnetTransactionProcessor.java while we do not know yet if it is maxFeePerGas that will be used. 
And we already calculate the valid value needed for upfrontgascost here https://github.com/hyperledger/besu/blob/3267501c8cd2a1cd116b8b295e5baedab12bd3b5/[…]erledger/besu/ethereum/mainnet/MainnetTransactionProcessor.java

This PR also fix somme issues regarding the transaction pool for eip1559 and a tracing issue

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-31 09:55:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2340" class=".btn">#2340</a>
            </td>
            <td>
                <b>
                    CMS creation/validation logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Added two main classes to handle CMS: `CmsCreator` and `CmsValidator`.

## Changelog

No changelog updated required at the moment.

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-31 03:55:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2339" class=".btn">#2339</a>
            </td>
            <td>
                <b>
                    use baseFee instead of baseFeePerGas for retesteth genesis config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

minor tweak to the baseFee config parameter for retesteth command since  that rpc command spec has not (yet?) changed to baseFeePerGas


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->



## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-29 04:06:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2338" class=".btn">#2338</a>
            </td>
            <td>
                <b>
                    Fix consensus vulnerability regarding excessively large 1559 fee fields
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
https://github.com/ethereum/pm/issues/321#issuecomment-850230251

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 18:08:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2335" class=".btn">#2335</a>
            </td>
            <td>
                <b>
                    update referencetests to latest develop branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
update referencetests to latest develop branch
get 1559 test cases passing
fix transaction encoding of 2718 typed transactions

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2229 
fixes #2285 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 01:42:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2334" class=".btn">#2334</a>
            </td>
            <td>
                <b>
                    GoQuorum ATs: ignore multiple private states tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Ignore new multiple private states (mps) tests

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 22:52:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2333" class=".btn">#2333</a>
            </td>
            <td>
                <b>
                    GoQuorum ATs: ignore spam test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Ignore (new) spam label since this test doesn't work well for EthSigner/Besu

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 20:51:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2324" class=".btn">#2324</a>
            </td>
            <td>
                <b>
                    Adds unrestricted privacy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Allows users to utilise unrestricted private transactions. This stores the private transaction in the data of the unrestricted privacy precompile address on-chain. The default implementation is unencrypted, further plugin extension points are required to allow the user to encrypt transactions on-chain. 

## mutually exclusive private restriction modes

### Privacy group state
You can not run a node in mixed `unrestricted`/`restricted` privacy modes. There are potential issues with private state and privacy groups. There is only one private state per group, consequently, you could have a mix of private transaction restriction types in the same group. Whilst it's not a problem per se it could lead to confusion and inconsistent state between nodes.

### Flexible privacy groups
Onchain privacy groups are not currently possible with unrestricted transactions.

### CLI options
`--privacy-enabled` and `--privacy-unrestricted-enabled` must be specified to enable this feature. 

## Changelog

- [ ] adds unrestricted privacy 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 13:18:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2322" class=".btn">#2322</a>
            </td>
            <td>
                <b>
                    Orion info in changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added Tessera/Orion info to changelog

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 23:25:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2321" class=".btn">#2321</a>
            </td>
            <td>
                <b>
                    Fix SECP256R1AcceptanceTest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel@io.builders>

## PR description

SECP256R1AcceptanceTest needed to set `SECP256R1` as signature algorithm instance. Because this variable is static and is used in `BesuNode` to [create a key pair](https://github.com/hyperledger/besu/blob/master/acceptance-tests/dsl/src/main/java/org/hyperledger/besu/tests/acceptance/dsl/node/BesuNode.java#L155) it could happen that other tests were using the SECP256R1 signature algorithm by accident becuase of this, depending on the order in which the tests were executed. This caused the acceptance tests to be flaky.
This PR introduces the possibility to set a pre-generated key pair in `BesuNodeFactory`. This allows to set a SECP256R1 key pair without changing `SignatureAlgorithmFactory.instance`, which avoids that other tests can happen to use SECP256R1 when they expect SECP256K1.

## Fixed Issue(s)
reintroduces test which was ignored in #2267 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 20:32:54 +0000 UTC
    </div>
</div>

