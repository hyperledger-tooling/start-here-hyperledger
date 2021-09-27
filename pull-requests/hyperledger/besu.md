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
                PR <a href="https://github.com/hyperledger/besu/pull/2810" class=".btn">#2810</a>
            </td>
            <td>
                <b>
                    Make ExceptionalHaltReason an interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrate ExceptionalHaltReason to an interface from an enum. The enum
made it difficult for downstream implementations to add custom reasons
as to why the EVM has halted. Switching to an interface is needed
because enums are final and not extensible.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 16:20:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2809" class=".btn">#2809</a>
            </td>
            <td>
                <b>
                    Jumpdest cache bits
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

Adds caching of valid jump destinations in a contract. This should reduce re-work previously required each time any function in the contract is called.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #2607 

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 14:58:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2807" class=".btn">#2807</a>
            </td>
            <td>
                <b>
                    Add QBFT support for evmtool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                ## PR description
Support QBFT in evmtool. #2749 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 06:03:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2806" class=".btn">#2806</a>
            </td>
            <td>
                <b>
                    Rename: OnChain -> onchain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rename refactor. Fixes #2750 

`find . -name '*.java' -type f -print0 | xargs -0 sed -i "" 's/onChain/onchain/g'`
Then I noticed "constructionChain" and "InstructionChain" so I changed them back:
`find . -name '*.java' -type f -print0 | xargs -0 sed -i "" 's/ionchain/ionChain/g'
`
`find . -name '*.java' -type f -print0 | xargs -0 sed -i "" 's/OnChain/Onchain/g'`
and change this RPC method name back
`find . -name '*.java' -type f -print0 | xargs -0 sed -i "" 's/privx_findOnchainPrivacyGroup/privx_findOnChainPrivacyGroup/g'
`
Then I had to move the several class files using IDE

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 04:14:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2805" class=".btn">#2805</a>
            </td>
            <td>
                <b>
                    reduce use of global quorum config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

The use of the org.hyperledger.besu.config.GoQuorumOptions static variable is ugly. In particular does changing its value during tests cause flaky tests. To ameliorate the issue this PR

- removes unused code that did rely on GoQuorumOptions
- removes access to GoQuorumOptions deep in the call stack by looking it up in the transaction validator instead
- change the TransactionDecoder to explicitly take the  goQuorumCompatbility flag as an argument where access to the  transaction validator is not easy
- rewriting all tests that did change the GoQuorumOptions by mocking  the option change instead.

Signed-off-by: Taccat Isid <taccatisid@protonmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2775.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-27 01:03:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2804" class=".btn">#2804</a>
            </td>
            <td>
                <b>
                    Raise Visibility of Constructor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Raise the visibility of AbstractCreateOperation's constructor to
protected from package so that create operations outside the library can
re-use the existing code.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-25 03:45:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2801" class=".btn">#2801</a>
            </td>
            <td>
                <b>
                    [#536] Add support for custom private key file for public-key export and public-key export-address commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR adds `--node-private-key-file` option to `public-key export-address` and `public-key export` commands.

## Fixed Issue(s)
Fixes #536

## Changelog

- [ ] Add support for custom private key file for public-key export and public-key export-address commands
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 20:32:45 +0000 UTC
    </div>
</div>

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

