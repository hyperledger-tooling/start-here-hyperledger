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
                PR <a href="https://github.com/hyperledger/besu/pull/2501" class=".btn">#2501</a>
            </td>
            <td>
                <b>
                    SECP256R1 BC now using non-deterministic variant
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

- Updated our `SignatureAlgorithm` interface with a method to return the K calculator implementation (BC)
- Each concrete implementation returns the expected calculator:
  - SECP256K1: deterministic calculator
  - SECP256R1: non-deterministic calculator

## Fixed Issue(s)
Fixes #2500

## Changelog
N/A
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 00:21:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2499" class=".btn">#2499</a>
            </td>
            <td>
                <b>
                    fix ropsten consensus issue
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

Fix a consensus issue detected on ropsten. There was a check of elasticity that seems to be related to old version of the specification. This made a double check of the elasticity in the code. I only kept the version that corresponds to the latest version of the spec.
>
		if INITIAL_FORK_BLOCK_NUMBER == block.number:
			expected_base_fee_per_gas = INITIAL_BASE_FEE
		elif parent_gas_used == parent_gas_target:
			expected_base_fee_per_gas = parent_base_fee_per_gas
		elif parent_gas_used > parent_gas_target:
			gas_used_delta = parent_gas_used - parent_gas_target
			base_fee_per_gas_delta = max(parent_base_fee_per_gas * gas_used_delta // parent_gas_target // BASE_FEE_MAX_CHANGE_DENOMINATOR, 1)
			expected_base_fee_per_gas = parent_base_fee_per_gas + base_fee_per_gas_delta
		else:
			gas_used_delta = parent_gas_target - parent_gas_used
			base_fee_per_gas_delta = parent_base_fee_per_gas * gas_used_delta // parent_gas_target // BASE_FEE_MAX_CHANGE_DENOMINATOR
			expected_base_fee_per_gas = max(parent_base_fee_per_gas - base_fee_per_gas_delta, 0)
		assert expected_base_fee_per_gas == block.base_fee_per_gas, 'invalid block: base fee not correct'


I also detected a code that seems invalid in the generation of expectedBaseFee (max missing)
> expected_base_fee_per_gas = max(parent_base_fee_per_gas - base_fee_per_gas_delta, 0)

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-05 12:26:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2497" class=".btn">#2497</a>
            </td>
            <td>
                <b>
                    [Issue 1975] Add option to require tx replay protection
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
Add new option (`--strict-tx-replay-protection-enabled`) to require locally submitted transaction to use transaction replay protection.  This option defaults to false for now, in the future we should change this to default to true. 

## Fixed Issue(s)
Fixes #1975

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-04 19:14:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2495" class=".btn">#2495</a>
            </td>
            <td>
                <b>
                    test simple poc blacklist peers
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
        Created At 2021-07-02 11:56:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2493" class=".btn">#2493</a>
            </td>
            <td>
                <b>
                    refcator response constructor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a non-functional change that sets me up to better support eth66.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 17:07:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2492" class=".btn">#2492</a>
            </td>
            <td>
                <b>
                    Fix bonsai storage inconsistency issue
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

This ticket fixes a consistency issue between the blockchain storage part and the worldstate storage .

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 12:46:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2491" class=".btn">#2491</a>
            </td>
            <td>
                <b>
                    enable quorum ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 00:05:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2490" class=".btn">#2490</a>
            </td>
            <td>
                <b>
                    GraphQL schema + adapter updates to handle GoQuorum transaction fields
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
Updates the GraphQL schema + adapter to handle GoQuorum transaction fields
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 12:53:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2489" class=".btn">#2489</a>
            </td>
            <td>
                <b>
                    Refactor: make it easier to locate private on-chain re-hydrate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make it easier to find where the re-hydrate happens when adding a new user to a group

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 11:48:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2487" class=".btn">#2487</a>
            </td>
            <td>
                <b>
                    QBFT release changelog entry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Frame <jasonwframe@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
QBFT release changelog entry

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 23:30:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2486" class=".btn">#2486</a>
            </td>
            <td>
                <b>
                    Add Early Return
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 22:07:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2485" class=".btn">#2485</a>
            </td>
            <td>
                <b>
                    Disconnect on Message Over 10MB
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
We've been benefitting from herd immunity from this. Time to join the herd.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 14:52:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2482" class=".btn">#2482</a>
            </td>
            <td>
                <b>
                    no trace for method calls in private tx simulator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Addresses memory issues with certain contracts in priv_call
See https://github.com/hyperledger/besu/issues/2387

No-op tracing implementation used everywhere in privacy. Tracing is not currently supported in privacy so no need for this overhead.

This NO_TRACING implementation is used by eth_call so it makes sense for this to be used by priv_call - and this explains the difference in memory usage between public and private states that users have reported.

ContainerTests all pass locally.
Customer provided tests in public and private execution also successful with this change. 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 04:01:03 +0000 UTC
    </div>
</div>

