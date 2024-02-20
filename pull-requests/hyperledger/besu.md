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
                PR <a href="https://github.com/hyperledger/besu/pull/6595" class=".btn">#6595</a>
            </td>
            <td>
                <b>
                    Extend and refactor transaction selection service
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
        Created At 2024-02-19 19:39:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6593" class=".btn">#6593</a>
            </td>
            <td>
                <b>
                    Increment private nonce even if transaction failed.
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
Fixes #1942 


Classes to follow:

BesuCommand
PrivateTransactionProcessor
PrivateMutableWorldStateUpdater
SimpleWorld
PrivacyParameters
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 11:40:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6592" class=".btn">#6592</a>
            </td>
            <td>
                <b>
                    Extend Blockchain service
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

Another PR after https://github.com/hyperledger/besu/pull/6584 that extend the data provided by a service, this time `Blockchain` service, these extensions are needed to introduce the new Transaction Simulation service.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 11:20:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6587" class=".btn">#6587</a>
            </td>
            <td>
                <b>
                    Mining Parameters Metrics
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
This PR adds metrics to the Mining Parameters `minGasPrice` and `minPriorityFee` as `ethereum_min_gas_price` and `ethereum_min_priority_fee` respectively to expose runtime Values of those properties set via cli arguments or RPC methods as a gauge.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
https://github.com/hyperledger/besu/issues/6291
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 02:48:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6585" class=".btn">#6585</a>
            </td>
            <td>
                <b>
                    Test results artifacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - corrects path on acceptanceTest
- adds direct gradle dependency from build to javadoc, fixes #6552 
- renames consolidation checks to separate from workflow names
- replaces unreliable test splitting action with bash script in reference tests
- corrects missing test target during unit tests
- embeds version number at release time, overriding gradle.properties value
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-17 02:04:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6584" class=".btn">#6584</a>
            </td>
            <td>
                <b>
                    Extend BesuConfiguration service
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

This PR adds a method to `BesuConfiguration` service get the current `minGasPrice`, in order to implement that a little refactoring was necessary, since services needs to be instantiated very early during the startup, since they need to be visible during the registration of the plugins, but at that stage most configurations are not yet ready, so there is now a separation between the instantiation and the initialization that is done after when the configuration is ready, the initialization is performed before the plugins start, so service are 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 17:45:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6582" class=".btn">#6582</a>
            </td>
            <td>
                <b>
                    Use Invalid payload attributes error code 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Return "invalid payload attributes" instead of "invalid params" if the payload attributes are, in fact, invalid

fixes #6554
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 06:50:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6581" class=".btn">#6581</a>
            </td>
            <td>
                <b>
                    feat: add `eth_blobBaseFee`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span><span class="chip">mainnet</span>
            </td>
            <td>
                ## PR description
Add `eth_blobBaseFee`

## Fixed Issue(s)
fixes #6579
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 03:47:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6578" class=".btn">#6578</a>
            </td>
            <td>
                <b>
                    fix: Discovery not taking nat manager port-mapping into account
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
Proposal to fix the issue i reported in #6573 
* `PingPacketData` should take into account the NATManager portMapping for the discoveryPort.
* Take into account the `udpPort` from the `PingPacketData` if the `host` is also taken from there.

## Fixed Issue(s)
fixes: https://github.com/hyperledger/besu/issues/6573
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 08:43:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6577" class=".btn">#6577</a>
            </td>
            <td>
                <b>
                    [MINOR] Use better savings estimate for x-trie-log prune
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following on from #6540, use `total-sst-files-size + total-blob-file-size` instead of `estimate-live-data-size` for x-trie-log prune estimate.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 04:26:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6576" class=".btn">#6576</a>
            </td>
            <td>
                <b>
                    Remove duplicated addCreate call
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
Remove duplicated call to the addCreate method. The method is already called here  https://github.com/hyperledger/besu/blob/5c295c5aa6c277287bf3c8d6679a9cca36427838/evm/src/main/java/org/hyperledger/besu/evm/processor/ContractCreationProcessor.java#L125
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 04:06:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6575" class=".btn">#6575</a>
            </td>
            <td>
                <b>
                    bump to 24.2.0-SNAPSHOT
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
post-release bump

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 00:20:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6574" class=".btn">#6574</a>
            </td>
            <td>
                <b>
                    Apply Reference tests v13.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Apply v 13.1 of the reference tests, includes test related fixes around initing the KZG precompile, uint64s in timestamps and blob gas, and some formatting cleanup.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 23:36:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6572" class=".btn">#6572</a>
            </td>
            <td>
                <b>
                    add curl in base openjdk-latest dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
As a user of the besu docker image I would like to have curl available in the running container.

NB: teku include curl in their image https://github.com/Consensys/teku/blob/b544b9ebe589e78fa2f075ae389b041dc2871ea2/docker/jdk21/Dockerfile#L17

## Fixed Issue(s)
fixes #6571
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 15:12:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6570" class=".btn">#6570</a>
            </td>
            <td>
                <b>
                    remove useless persist during backward sync
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

During backward sync we call validateAndProcessBlock, which will process the block, update the state, and calculate the root hash.

If the block is validated, we will persist the block again for no reason, which will lead to a new unnecessary calculation of rootHash. Removing this second call should really significantly improve performance.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 14:28:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6568" class=".btn">#6568</a>
            </td>
            <td>
                <b>
                    Add tests for user profiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                Add tests to ensure that the profiles are sensible and besu will start with each of them

Refs #6323
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 04:25:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6563" class=".btn">#6563</a>
            </td>
            <td>
                <b>
                    Fix for tx incorrectly discarded when there is a timeout during block creation
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

In case the selection of transactions during block creation goes in timeout, it is possible that some txs are incorrectly dropped from the txpool, since marked as invalid.
When the timeout occurs the block is created with all the txs selected until that moment, after that the world state is closed, while it is possible that a tx was still processing, in that case the processing tx validation could fail due fact that is no more possible to get the account from the closed world state, and the tx is wrongly tagged as invalid with UPFRONT_COST_EXCEED_BALANCE, that cause the tx to be dropped from the pool.

This PR, improves the handling of timeout and not selected txs, avoiding that them can be incorrectly dropped in case of timeout

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 13:37:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6562" class=".btn">#6562</a>
            </td>
            <td>
                <b>
                    feat: add fixed basefee options
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
Add `fixedBaseFee` options to forced `baseFee` same as `gasPrice` value.


I'm new to the Java language, please guide any aspects I can further improve or modify.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
https://github.com/hyperledger/besu/issues/6335
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 11:15:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6561" class=".btn">#6561</a>
            </td>
            <td>
                <b>
                    Bonsai limit trie logs enabled true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ux</span>
            </td>
            <td>
                Swap default value for --Xbonsai-limit-trie-logs-enabled from false to true

Also added a fallback value for the option (otherwise specifying --Xbonsai-limit-trie-logs-enabled on the command line, without a value, has the opposite effect

builds on #6536 

This option is not yet documented so no docs changes required.

Breaking change
The limit is now enabled by default. If you do not want the limit enabled, you need to explicitly set it to false
--Xbonsai-limit-trie-logs-enabled=false
However - the default is set to 512 which should work for most use cases.

fixes #6560

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 04:19:29 +0000 UTC
    </div>
</div>

