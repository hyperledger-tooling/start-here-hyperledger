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
                PR <a href="https://github.com/hyperledger/besu/pull/3114" class=".btn">#3114</a>
            </td>
            <td>
                <b>
                    Reduce log level down to debug on EthPeer Permissioning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reduce log level down to debug on EthPeer Permissioning - the logs can become very verbose when blocking p2p transactions in private networks.

Signed-off-by: Antony Denyer <git@antonydenyer.co.uk>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 16:04:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3112" class=".btn">#3112</a>
            </td>
            <td>
                <b>
                    Include invalid value in Enode error message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Makes it much easier for users to identify their mistake if the CLI argument after `--bootnodes <some-valid-enode>` has a typo. PicoCLI will treat any unrecognised option as another bootnode so it's very confusing to get an invalid enode message when the enode is fine and it's the next argument that's incorrect.

For example `--bootnodes enode://blah@127.0.0.1:30303 --datapath foo` would otherwise print an error message saying there wasn't an `enode://` prefix when there clearly is.  When the invalid value is shown the user can see that it's actually `--datapath` that's unrecognised and fix the problem.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 09:37:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3111" class=".btn">#3111</a>
            </td>
            <td>
                <b>
                    Eip 4399
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

Implements EIP-4399 by repurposing the DIFFICULTY opcode to provide entropy provided by beacon chain post merge.

This is intended to change the behavior during the merge, and leaving the semantic changes to clarify this behavior till after the merge, when the opcode can be documented as renamed to RANDOM, thought its instruction byte remains the same.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-28 04:50:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3110" class=".btn">#3110</a>
            </td>
            <td>
                <b>
                    Removing deprecated hash variable which was used to cache the transaction
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
#2937 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 14:22:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3109" class=".btn">#3109</a>
            </td>
            <td>
                <b>
                    Updating gradle to version 7.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                check the [release notes](https://docs.gradle.org/7.3/release-notes.html) to see what is new (jdk17 support among other things).

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 13:35:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3108" class=".btn">#3108</a>
            </td>
            <td>
                <b>
                    Rename BftForksSchedule to ForksSchedule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Preparation for https://github.com/hyperledger/besu/pull/3097

* Rename BftForksSchedule to ForkSchedule
* Make ForksSchedule generic beyond BftConfigOptions to allow it to work for MiningCoordinator
* Rename static factory to make it specific to BftConfigOptions
* Move ForksSchedule to common package

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 11:05:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3107" class=".btn">#3107</a>
            </td>
            <td>
                <b>
                    Merge: engine_getPayload json-rpc endpoint
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
Merge json-rpc endpoint for `engine_getPayload` from the merge feature branch.

Addresses part of #2965 


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 18:59:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3106" class=".btn">#3106</a>
            </td>
            <td>
                <b>
                    Remove Ethsigner to Besu acceptance tests
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
Remove EthSigner acceptance tests as these test cases are covered in EthSigner and other test tools.

FYI @jflo
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 01:13:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3105" class=".btn">#3105</a>
            </td>
            <td>
                <b>
                    Tls configuration
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

Adding two new options:
* `--rpc-http-tls-protocols` to be able to specify TLS protocol version 
* `--rpc-http-tls-ciphersuites` to be able to specify Java cypher suites


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes [#474](https://github.com/hyperledger/besu/issues/474): 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 13:12:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3104" class=".btn">#3104</a>
            </td>
            <td>
                <b>
                    merge of Blockheader changes to support random field
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
In support of [EIP-4399](https://github.com/ethereum/EIPs/blob/979cf123558bab61e2278f3c962c9a68d1adc2f4/EIPS/eip-4399.md) this PR adds a field to block headers, `random` which is 32 bytes of randao randomness data.

In accordance with spec, we re-purpose mixHash as random in RLP encoding and decoding, since they should be mutually exclusive -  a block with `random`  will not have a `mixHash` and vice-versa

related to #2897 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 08:04:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3103" class=".btn">#3103</a>
            </td>
            <td>
                <b>
                    (internal) Refactor PrivacyReorgTest to use mock enclave
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
PrivacyReorgTest currently spins up a Orion instance just to store and retrieve the same private payload - this PR refactors it into a mock enclave.

## Fixed Issue(s)
fixes #3083 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 04:34:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3101" class=".btn">#3101</a>
            </td>
            <td>
                <b>
                    Prepare to merge execute_getPayload json-rpc endpoint into main
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

minor refactor in support of merging getPayload rpc method into main
* ensure we always serialize as even length hex representation
* move payload id into consensus namespace
* remove unused protocolSchedule

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 23:32:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3100" class=".btn">#3100</a>
            </td>
            <td>
                <b>
                    Jiri maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                JIri has made [significant commits](https://github.com/hyperledger/besu/pulls?q=is%3Apr+author%3Agezero) improving the quality and features of besu, this PR adds him as a maintainer.

Voting ends 2 weeks from the publication of this PR or once a majority of the maintainers vote.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 19:16:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3098" class=".btn">#3098</a>
            </td>
            <td>
                <b>
                    Migration mining coordinator duplicate event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Split out from https://github.com/hyperledger/besu/pull/3097 as it's a non-breaking issue. (But still part of https://github.com/hyperledger/besu/issues/2999)

Changes from siladu:migration-mining-coordinator viewable here: https://github.com/siladu/besu/compare/migration-mining-coordinator...migration-mining-coordinator_duplicate-event

The issue is that both SchedulableMiningCoordinator and its delegate, BftMiningCoordinator are registered as BlockAddedObservers when the mining coordinator is started. 
This means a duplicate event is processed:
```
DEBUG | BaseBftController | New chain head detected (block number=1), currently mining on top of 0.
DEBUG | BaseBftController | New chain head detected (block number=1), currently mining on top of 1.
TRACE | BaseBftController | Discarding duplicate NewChainHead event. chainHeight=1 
```

It is correctly discarded so it's not a blocker, but it should still be fixed.

I decided to cover this only using unit tests.
I considered the qbft integration-tests, but they avoid executing the mining coordinator, instead requiring the test code to 'manually' do the coordination.
This fix also seemed too fined grained for an acceptance test.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 14:21:49 +0000 UTC
    </div>
</div>

