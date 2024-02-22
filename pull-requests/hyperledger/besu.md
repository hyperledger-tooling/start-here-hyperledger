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
                PR <a href="https://github.com/hyperledger/besu/pull/6600" class=".btn">#6600</a>
            </td>
            <td>
                <b>
                    Gha docker pull
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Most advanced CI tests are deferred until PR approval, but you could:

- [x] locally run all unit tests via: `./gradlew build`
- [x] locally run all acceptance tests via: `./gradlew acceptanceTest`
- [x] locally run all integration tests via: `./gradlew integrationTest`
- [x] locally run all reference tests via: `./gradlew ethereum:referenceTests:referenceTests`


## PR description

Now appends the correct docker pull command to the release notes, i.e.

`docker pull ghcr.io/hyperledger/besu:24.2.0-RC1`

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 16:17:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6599" class=".btn">#6599</a>
            </td>
            <td>
                <b>
                    Ensure halt reasons in TraceFrames in `DebugOperationTracer.tracePostExecution`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This PR fixes the debug trace series generation for `opcodes` that do not set an explicit `ExceptionalHaltReason` in the `OperationResult`. Previously, operations like `dup5` could lead to an exceptional halt (e.g., due to running out of gas) without this being accurately captured in the trace output, as the halt reason was not set explicitly. This situation affected the `FlatTraceGenerator's` ability to accurately reflect halt conditions and `subtrace` counts.

The `DebugOperationTracer.tracePostExecution` method has been updated to check the `MessageFrame` for an exceptional halt reason if it's absent in the `OperationResult`. This adjustment aligns with the existing approach used by the `StandardJsonTracer`

The trace output for the transaction referenced in the [issue](https://github.com/hyperledger/besu/issues/6591) now accurately displays the correct halt reason and appropriately counts subtraces.

```diff
{
   "jsonrpc":"2.0",
   "id":1,
   "result":[
      {
         "action":{
            "callType":"call",
            "from":"0xd8422593f16cd6d65c3f4cfa28b5b5a862037123",
            "gas":"0x1a18",
            "input":"0x5b7d7482000000000000000000000000000000000000000000000000000000000000004000000000000000000000000000000000000000000000000000000000000000a0000000000000000000000000000000000000000000000000000000000000004034313465376364326235656636313337656166383661396134653064666430333536313063323562323536333031633662396361356361313531653233373965000000000000000000000000000000000000000000000000000000000000004034646163313738646333376331303736346235643862373862633135323635366437316662343865626537396361613835343437336530663031313132313732",
            "to":"0xd1a3abf42f9e66be86cfdea8c5c2c74f041c5e14",
            "value":"0x0"
         },
         "blockHash":"0x2345afc92f072449294eba81a33116da5d014e74ecbe5db53e5d72b40145976f",
         "blockNumber":2160351,
-        "result": {
-           "gasUsed": "0x0",
-           "output": "0x"
-        },
-        "subtraces": 0,
+       "error":"Out of gas",
+       "subtraces":1,
        "traceAddress":[
            
         ],
         "transactionHash":"0xea89b8082ab1e9e8f0a025ead197ce8e2cdf4b1212d4ec13a91e97570485a053",
         "transactionPosition":0,
         "type":"call"
      },
      {
         "action":{
            "callType":"delegatecall",
            "from":"0xd1a3abf42f9e66be86cfdea8c5c2c74f041c5e14",
            "gas":"0x6dd",
            "input":"0x5b7d7482000000000000000000000000000000000000000000000000000000000000004000000000000000000000000000000000000000000000000000000000000000a0000000000000000000000000000000000000000000000000000000000000004034313465376364326235656636313337656166383661396134653064666430333536313063323562323536333031633662396361356361313531653233373965000000000000000000000000000000000000000000000000000000000000004034646163313738646333376331303736346235643862373862633135323635366437316662343865626537396361613835343437336530663031313132313732",
            "to":"0x564477025731ee7197eecf2c4a0d0106cc3e4572",
            "value":"0x0"
         },
         "blockHash":"0x2345afc92f072449294eba81a33116da5d014e74ecbe5db53e5d72b40145976f",
         "blockNumber":2160351,
-        "result": {
-           "gasUsed": "0xffffffffffffece0",
-            "output": "0x"
-         },
+       "error":"Out of gas",
         "subtraces":0,
         "traceAddress":[
            0
         ],
         "transactionHash":"0xea89b8082ab1e9e8f0a025ead197ce8e2cdf4b1212d4ec13a91e97570485a053",
         "transactionPosition":0,
         "type":"call"
      }
   ]
}

```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 04:41:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6598" class=".btn">#6598</a>
            </td>
            <td>
                <b>
                    PR Template updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - replaces comment on PR with template like the one used for opening an issue.
- makes test workflows manually runnable via workflow_dispatch
- updates to latest version of gradle build action
- corrects login to ghcr on nightly builds
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 02:33:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6596" class=".btn">#6596</a>
            </td>
            <td>
                <b>
                    Clique block period transition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 07:34:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6595" class=".btn">#6595</a>
            </td>
            <td>
                <b>
                    Refactor `TransactionSelectionService`
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

Scope of this refactor is to move the `TransacationSelectionService` from protocol context to mining parameters where it is more pertinent

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

