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
                PR <a href="https://github.com/hyperledger/besu/pull/5011" class=".btn">#5011</a>
            </td>
            <td>
                <b>
                    DebugGetRawBlock and DebugGetRawHeader missing methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span>
            </td>
            <td>
                ## PR description
Adds two missing methods as per [api-documentation](https://ethereum.github.io/execution-apis/api-documentation/):

- DebugGetRawBlock - Returns an RLP-encoded block.
- DebugGetRawHeader - Returns an RLP-encoded header.

**Fixes hive tests:**

- debug_getRawBlock/get-block-n (besu) 
- debug_getRawBlock/get-genesis (besu) 
- debug_getRawBlock/get-invalid-number (besu) 
- debug_getRawHeader/get-block-n (besu) 
- debug_getRawHeader/get-genesis (besu) 
- debug_getRawHeader/get-invalid-number (besu)

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 20:28:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5009" class=".btn">#5009</a>
            </td>
            <td>
                <b>
                    Simplify protocolSchedule query
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to referencetests/evmtool, @shemnon did this: https://github.com/hyperledger/besu/commit/a080bffcbab3d4cd9f9a264285f6b0c39b53a54b

If we revert this, withdrawals referencetests still pass so I think it's the right thing to do.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 16:08:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5008" class=".btn">#5008</a>
            </td>
            <td>
                <b>
                    adding test for nonblob blob transaction
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
        Created At 2023-01-26 16:07:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5007" class=".btn">#5007</a>
            </td>
            <td>
                <b>
                    Allow blob tx in Cancun
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 14:48:04 +0000 UTC
    </div>
</div>

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

