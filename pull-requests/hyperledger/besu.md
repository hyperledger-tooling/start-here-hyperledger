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
                PR <a href="https://github.com/hyperledger/besu/pull/2796" class=".btn">#2796</a>
            </td>
            <td>
                <b>
                    Evm speedup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Broad reaching optimizations to speed up EVM calculations
* Generally speaking, use `int` and `long` where it is more appropriate than `UInt256` (memory indexes mostly)
* Move the internal stack to `Bytes` from `UInt256`
* Re-work the flow of many operations to account for the above

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 14:57:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2793" class=".btn">#2793</a>
            </td>
            <td>
                <b>
                    Feature/merge consensus validated
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

* implement consensusValidated
* implement forkChoiceUpdated
* add Merge specific implementations of:
  * BlockValidator
  * BlockProcessor 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes [merge-477](https://github.com/ConsenSys/protocol-misc/issues/477)
fixes [merge-478](https://github.com/ConsenSys/protocol-misc/issues/478)

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 00:23:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2792" class=".btn">#2792</a>
            </td>
            <td>
                <b>
                    Alternative proposal for breaking change to the way plugins load cli options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://wiki.hyperledger.org/display/BESU/DRAFT+-+Pico+CLI+Plugin+Integration

The main change is to move preparePlugins into the begging of the run method. This means that all the cli parsing will happen before the method register is called. 

The only way to register cli options is to use the extra hook provided by `BesuPlugins::registerPicoCLIOptions`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 13:17:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2790" class=".btn">#2790</a>
            </td>
            <td>
                <b>
                    Evm move
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move the EVM classes to a standalone module. This is mostly moves but
some API re-design to peel out some features not essential to the EVM,
such as privacy support and ties to the data storage subsystem.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 07:02:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2789" class=".btn">#2789</a>
            </td>
            <td>
                <b>
                    Rollback TransactionGasCalculator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rollback the transactionGasCalculator changes. This was done in
preparation for the EVM modularization.  Instead, destructure the data
needed to calculate the gas instead of passing in the whole transaction.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 05:15:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2788" class=".btn">#2788</a>
            </td>
            <td>
                <b>
                    IBFT and QBFT to use a tolerance on minimum seconds between blocks in header validation rule
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
In IBFT and QBFT it is possible in some circumstances for a block to be created with a timestamp less than the specified block period. This add an optional tolerance to the header validation rule that the blocks must be at least x seconds than the parent block to allow for this. Without this change it might not possible to sync or import an existing IBFT chain that has this issue.

There will be work in another PR to fix the circumstances under which this can occur.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 03:44:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2787" class=".btn">#2787</a>
            </td>
            <td>
                <b>
                    Merge main
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

merge main in.  In PR form to ensure CI passes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 03:27:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2784" class=".btn">#2784</a>
            </td>
            <td>
                <b>
                    Allow the use of BESU_CONFIG_FILE env var
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                ## PR description
Enable the use of environment variable `BESU_CONFIG_FILE` to specify config toml

## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/2455

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 13:41:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2783" class=".btn">#2783</a>
            </td>
            <td>
                <b>
                    Snapsync get list  of accounts in range
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 08:14:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2782" class=".btn">#2782</a>
            </td>
            <td>
                <b>
                    Feature/merge execute payload
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
* implements engine_executePayload
* rename and repurpose rayonism options & flag
* treat the merge as another consensus mechanism:
  * add a `merge` consensus gradle subproject 
  * create MergeBesuController
  * create MergeProtocolSchedule 
  * create MergeContext for merge-specific consensus context
  * create MergeHeaderValidationRuleFactory for merge specific header validation rules
  * create MergeUnfinalizedValidationRule, attempt to enforce finalized block rules for import


## Fixed Issue(s)
protocol-misc 476 
protocol-misc 485

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 06:00:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2779" class=".btn">#2779</a>
            </td>
            <td>
                <b>
                    Create new datatypes module for Address, Hash, and Wei
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Create a new `datatypes` module to hold datatypes that are broadly used.
This will aid modularization by making sure the base types in the module
minimize the amount of unrelated support classes needed.

Move the Address, Hash, and Wei to datatypes in as they are needed for
EVM modularization.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 14:34:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2774" class=".btn">#2774</a>
            </td>
            <td>
                <b>
                    fix RC1-SNAPSHOT release version 🤦‍♂️
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
add missing -SNAPSHOT to gradle.properties build version

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 19:12:07 +0000 UTC
    </div>
</div>

