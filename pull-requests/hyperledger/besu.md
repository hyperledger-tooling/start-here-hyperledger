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
                PR <a href="https://github.com/hyperledger/besu/pull/5892" class=".btn">#5892</a>
            </td>
            <td>
                <b>
                    Add updated storage to evmtool json trace
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

Add the EIP-3155 "storage" option to the standard tracer, with the caveat only updated storage is logged.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 03:27:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5891" class=".btn">#5891</a>
            </td>
            <td>
                <b>
                    add plugin API to enable plugins to validate transaction before they are added to the transaction pool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Adding a plugin API to enable plugins to validate of transactions entering the transaction pool
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 00:41:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5890" class=".btn">#5890</a>
            </td>
            <td>
                <b>
                    Update holesky with fixed extraData, genesis time, shanghaiTime
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Incorporates https://github.com/eth-clients/holesky/pull/73
and also @fab-10's changes from https://github.com/eth-clients/holesky/pull/72
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 21:44:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5889" class=".btn">#5889</a>
            </td>
            <td>
                <b>
                    Draft PR: Code storage by hash
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
Draft PR for storing code by hash instead of by address. This is needed snapsync as we need to be able to retrieve the code by hash.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixed #5388 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 07:02:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5887" class=".btn">#5887</a>
            </td>
            <td>
                <b>
                    SnapServer using FlatDB Strategy
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
Draft PR to implement SnapServer using FlatDB Strategy

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3165 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-16 12:49:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5886" class=".btn">#5886</a>
            </td>
            <td>
                <b>
                    Fix: correctly convert percentage options in TOML configuration file
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

Fix for a regression introduced by #5772 that causes the following exception when the option `tx-pool-limit-by-account-percentage` is defined as a number in the configuration file

```
TomlInvalidTypeException: Value of 'tx-pool-limit-by-account-percentage' is a float while processing argument at or before arg[0] '--config-file=./config.toml' in [--config-file=./config.toml]: org.apache.tuweni.toml.TomlInvalidTypeException: Value of 'tx-pool-limit-by-account-percentage' is a float
```

the fix is to simply convert percentage options to string when parsing the file
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 13:04:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5885" class=".btn">#5885</a>
            </td>
            <td>
                <b>
                    RPC - Implement Debug trace call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span><span class="chip">mainnet</span><span class="chip">RPC</span>
            </td>
            <td>
                ## PR description
Implement Debug trace call

## Fixed Issue(s)
fix #5747
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 09:05:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5884" class=".btn">#5884</a>
            </td>
            <td>
                <b>
                    EIP7516 - Add BlobBaseFee opcode to Cancun EVM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add BLOBBASEFEE to Cancun EVM

## Fixed Issue(s)
fixes #5869 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 05:59:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5883" class=".btn">#5883</a>
            </td>
            <td>
                <b>
                    [MINOR] test RLP used for encode/decode blob tx should contain to field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `to` field cannot be empty for blob tx so it doesn't make sense to check encoding / decoding without this

However that field being absent doesn't fail the tests because this is checked in the transaction validation -   https://github.com/hyperledger/besu/blob/4b2ef689c1f64e3fdb293dec826af1ad57e54fca/ethereum/core/src/main/java/org/hyperledger/besu/ethereum/mainnet/MainnetTransactionValidator.java#L299


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 02:49:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5882" class=".btn">#5882</a>
            </td>
            <td>
                <b>
                    [DO NOT MERGE] devnet8: correct address and modulus for beacon root
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Do not merge. This is a short time brach for devnet 8.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 23:28:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5880" class=".btn">#5880</a>
            </td>
            <td>
                <b>
                    display only peers ready for requets on ethstats
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Filter peer collection by those ready for connection. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 13:04:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5879" class=".btn">#5879</a>
            </td>
            <td>
                <b>
                    Tune G1GC to reduce Besu memory footprint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

These flags have been suggested by @ahamlat , and we tested them for months now, they have the effect of reducing the off heap memory used by Besu, without affecting the overall performance.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 10:45:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5876" class=".btn">#5876</a>
            </td>
            <td>
                <b>
                    adds Matthew Whitehead as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I propose to add  @matthew1001 as a Besu project maintainer.

@matthew1001 contributed with many high quality commits:

- has implemented new JSON-RPC api endpoints, per execution api specs
- has improved error reporting in apis
- has improved configurability for non PoS networks

Here are [their past contributions on Besu project](https://github.com/hyperledger/besu/pulls?q=is:pr+author:matthew1001+is:closed).

Voting ends two weeks from today.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 17:20:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5875" class=".btn">#5875</a>
            </td>
            <td>
                <b>
                    init checkpoint state
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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 17:06:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5872" class=".btn">#5872</a>
            </td>
            <td>
                <b>
                    payload attributes: fix wrong warning and fail if beacon root is available before cancun
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
A wrong warning was logged when a payload attribute was sent before cancun.
Instead the validation of the payload attribute should fail if the parent beacon block root hash is available before cancun.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 04:06:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5871" class=".btn">#5871</a>
            </td>
            <td>
                <b>
                    #5868: fix beacon root address and modulus for devnet 9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
For the upcoming cancun devnet 9 the address and the modulus for EIP 4788 (parent beacon block root) have been changed. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 02:38:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5870" class=".btn">#5870</a>
            </td>
            <td>
                <b>
                    updated gradle verification metadata to fix spotless
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                regenerated the metadata file from scratch. Resulting in deletions of all old unused versions. Commands used:

```
rm gradle/verification-metadata.xml
./gradlew clean --write-verification-metadata sha256 spotlessCheck compileTestJava compileJava
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 02:22:19 +0000 UTC
    </div>
</div>

