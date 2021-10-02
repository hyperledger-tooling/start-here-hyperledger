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
                PR <a href="https://github.com/hyperledger/besu/pull/2815" class=".btn">#2815</a>
            </td>
            <td>
                <b>
                    Refactor(Balance/Ext-*Operations): Extract gas calculation into separate function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
* Extract gas cost calculation for Balance, ExtCodeCopy, ExtCodeHash, ExtCodeSize operations into `cost` function.
* Allow `cost` function to be called outside library

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 10:06:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2814" class=".btn">#2814</a>
            </td>
            <td>
                <b>
                    QBFT to log warning when using validator contract if genesis extra data has validator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also prevent existing warning from logging when using validator contract with no signers in genesis extra data.

Fixes https://github.com/hyperledger/besu/issues/2744
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 08:35:36 +0000 UTC
    </div>
</div>

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

