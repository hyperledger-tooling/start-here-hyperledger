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
                PR <a href="https://github.com/hyperledger/besu/pull/2505" class=".btn">#2505</a>
            </td>
            <td>
                <b>
                    Prioritize with nonce distance
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

Prevent multiple transactions from the same address from evicting others which are waiting in a full transaction pool. When we have to evict a transaction from a full pool, we now also consider how far it is from the lowest nonce from the same address already in the pool. We are also increasing the size of the pending transaction pool, so it should support the new 10MB maximum message size previously introduced by pr [#2485](https://github.com/hyperledger/besu/pull/2485) .

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog
Default value for `--tx-pool-max-size`  is now 32K.
- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 20:24:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2504" class=".btn">#2504</a>
            </td>
            <td>
                <b>
                    added london block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin.florentine@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
Adds protocol hardfork to London.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 17:58:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2502" class=".btn">#2502</a>
            </td>
            <td>
                <b>
                    Fix cleared storage issue
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
        Created At 2021-07-06 14:17:13 +0000 UTC
    </div>
</div>

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


## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-05 12:26:36 +0000 UTC
    </div>
</div>

