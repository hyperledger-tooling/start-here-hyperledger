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
                PR <a href="https://github.com/hyperledger/besu/pull/2822" class=".btn">#2822</a>
            </td>
            <td>
                <b>
                    Feature/merge get payload
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
in support of test mergenet:
 * add MergeBlockCreator
 * remove some of the rayonism hacks

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
addresses merge-488

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 23:15:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2821" class=".btn">#2821</a>
            </td>
            <td>
                <b>
                    Jumpdest constructor inj
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
Alternate implementation of [this PR](https://github.com/hyperledger/besu/pull/2809), which does not require a singleton for the jumpdest cache.
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
        Created At 2021-09-29 15:19:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2820" class=".btn">#2820</a>
            </td>
            <td>
                <b>
                    test benchmark CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Taccat Isid <taccatisid@protonmail.com>

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
        Created At 2021-09-29 01:47:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2819" class=".btn">#2819</a>
            </td>
            <td>
                <b>
                    added trace logging for ip -> dns when checking smart contract permissioning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>
Added some logging so users can see more details on what is being resolved and what is being rejected/permitted with regard to IP and DNS versions of enode. This will help when troubleshooting DNS + permissioning.

```
2021-09-29 11:08:50.183+10:00 | vert.x-eventloop-thread-2 | TRACE | NodePermissioningController | Node permissioning: Checking enode://3548c87b9920ff16aa4bdcf01c85f25117a29ae1574d759bad48cc9463d8e9f7c3c1d1e9fb0d28e73898951f90e02714abb770fd6d22e90371882a45658800e9@127.0.0.1:40404 -> enode://fcbe9f83218487b3c0b50878193880e6c25cfd86708c0a0bf0ca91f0ce633746a892fe240afa5b9a880b8bca48e8a22704ef937fdda2d7cc63e4d41ed1b417ae@127.0.0.1:30303
2021-09-29 11:08:50.186+10:00 | vert.x-eventloop-thread-2 | INFO  | NodeSmartContractV2PermissioningController | Permitted? false for IP enode://3548c87b9920ff16aa4bdcf01c85f25117a29ae1574d759bad48cc9463d8e9f7c3c1d1e9fb0d28e73898951f90e02714abb770fd6d22e90371882a45658800e9@127.0.0.1:40404
2021-09-29 11:08:50.189+10:00 | vert.x-eventloop-thread-2 | INFO  | NodeSmartContractV2PermissioningController | Permitted? false for DNS enode://3548c87b9920ff16aa4bdcf01c85f25117a29ae1574d759bad48cc9463d8e9f7c3c1d1e9fb0d28e73898951f90e02714abb770fd6d22e90371882a45658800e9@localhost:40404
2021-09-29 11:08:50.190+10:00 | vert.x-eventloop-thread-2 | TRACE | NodePermissioningController | Node permissioning - NodeSmartContractV2PermissioningController: Rejected enode://3548c87b9920ff16aa4bdcf01c85f25117a29ae1574d759bad48cc9463d8e9f7c3c1d1e9fb0d28e73898951f90e02714abb770fd6d22e90371882a45658800e9@127.0.0.1:40404 -> enode://fcbe9f83218487b3c0b50878193880e6c25cfd86708c0a0bf0ca91f0ce633746a892fe240afa5b9a880b8bca48e8a22704ef937fdda2d7cc63e4d41ed1b417ae@127.0.0.1:30303
```

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 01:13:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2818" class=".btn">#2818</a>
            </td>
            <td>
                <b>
                    Rename: OffChain -> offchain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

We are treating "offchain" as a single word.
Rename refactor. See #2750 for "onchain" change

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 00:15:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2817" class=".btn">#2817</a>
            </td>
            <td>
                <b>
                    Qbft RPCs should be disabled after starting with or switching to use validator contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Still TODO: manually test transitions and work out if any ITs or ATs are required**

## PR description

Qbft RPCs should be disabled after starting with or switching to use validator contract
Signer metrics and getValidatorsByBlock... should remain enabled.

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/2795

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 19:45:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2816" class=".btn">#2816</a>
            </td>
            <td>
                <b>
                    fix: private contracts not able to call public contracts that call other public contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Private contracts not able to call public contracts that call other public contracts. 

The root cause is that during `transferValue` the `MessageCallProcessor` attempts to get a mutable account. At this point the evm throws an exception as it is rightly not mutable!

This can be avoided in situations when there is no value to transfer.

## Fixed Issue(s)
fix #2803 Private Transaction Failed when invoking a Public Contract that calls another Public Contract


## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 15:26:19 +0000 UTC
    </div>
</div>

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

