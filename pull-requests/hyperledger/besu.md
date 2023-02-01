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
                PR <a href="https://github.com/hyperledger/besu/pull/5005" class=".btn">#5005</a>
            </td>
            <td>
                <b>
                    Address witdrawals failures in execution-spec-tests
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
Address withdrawal failures in [execution-spec-tests](https://github.com/ethereum/execution-spec-tests/tree/main/fillers/withdrawals):

```
large_withdrawals.json
withdrawals_balance_within_block.json
withdrawals_many_withdrawals.json
withdrawals_multiple_withdrawals_same_address.json
withdrawals_newly_created_contract.json
withdrawals_no_evm_execution.json
withdrawals_overflowing_balance.json
withdrawals_self_destructing_account.json
withdrawals_use_value_in_contract.json
withdrawals_use_value_in_tx.json
withdrawals_zero_amount.json
```
Not adding unit test coverage as these will be moved out of the `EIPTests` and reference tests soon.  

All tests pass when running with [EIPTests.bc4895](https://github.com/hyperledger/besu/blob/main/ethereum/referencetests/src/reference-test/java/org/hyperledger/besu/ethereum/vm/BlockchainReferenceTestTools.java#L86) enabled.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4934 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 13:04:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5003" class=".btn">#5003</a>
            </td>
            <td>
                <b>
                    Adding trace logs to mention ssz transaction encoding/deconding in logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 08:18:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5001" class=".btn">#5001</a>
            </td>
            <td>
                <b>
                    Revert "parallelization for unit tests (#5000)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit b22a52a88e42a5c11f0564f1c9603bff55687e9e.

Signed-off-by: Sally MacFarlane <macfarla.github@gmail.com>

It seems not all tests are running. Needs more investigation.

See #4921 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-25 06:36:10 +0000 UTC
    </div>
</div>

