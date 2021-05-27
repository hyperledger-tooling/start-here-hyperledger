---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/145" class=".btn">#145</a>
            </td>
            <td>
                <b>
                    Add examples/sabre_command to justfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is required to catch build, lint, and testing errors in this
example crate.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 17:03:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    Remove env output from 'just build'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is undesirable output when running the command in the developer workflow.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 16:59:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/143" class=".btn">#143</a>
            </td>
            <td>
                <b>
                    Update Sha2::Sha512 usage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update to work with the current version of sha2 used in transact.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 16:58:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/142" class=".btn">#142</a>
            </td>
            <td>
                <b>
                    TooManyRequests response bug fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes a bug in the recent update to handle `TooManyRequests`. Previously if control-c was pressed while the `slow_rate` method was attempting to resubmit a batch the workload would not stop until `slow_rate` had returned and it would usually result in a panic caused by a divide by zero error.

The following changes are added in this PR to fix this bug:
- After each time `slow_rate` is called the time and total batches counters used to calculate the effective submission rate are reset
- The `slow_rate` method is updated to default to 1 second of sleep if the effective rate is calculated to be 0, this avoids any possible divide by zero errors that were possible before
- A `receiver` argument is added to the `slow_rate` method, the method uses the receiver to check if a shutdown message has been sent each time it loops
- The `slow_rate` method is updated to return a boolean representing whether or not a shutdown message was sent. If `slow_rate` returns `true` the loop will break and the workload will stop

### **Testing:**
1. Start two splinter nodes with the experimental feature "back-pressure"
2. Create a circuit between the nodes, ensure that the scabbard version is set to 2 when creating the circuit
3. Use scabbard CLI to upload the smallbank smart contract
4. Use the transact CLI to start a smallbank workload, for example:
```
transact workload --targets http://localhost:8085/scabbard/<circuit-id>/<service-id> \
--key <private-key-path> \
--target-rate 5 \
--update 2 \
--workload smallbank \
-vv
```
5. Control-c immediately after seeing the log message:
```Received TooManyRequests message from target, attempting to resubmit batch```
check that the log shows:
```
Shutting down worker Smallbank-Workload-0
Worker received shutdown
```
and the workload stops
6. Run the workload command again
7. Control-c while batches are being successfully submitted
check that the same shutdown log message shows:
```
Shutting down worker Smallbank-Workload-0
Worker received shutdown
```
and the workload stops
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 21:58:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/140" class=".btn">#140</a>
            </td>
            <td>
                <b>
                    Create command workload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR creates a Command family workload that can be run using the `transact workload` CLI command

- Add `command` as a workload type to the transact workload subcommand
- Update WorkloadAction to handle command workloads
- Implement `CommandGeneratingIter`, `CommandTransactionWorkload` and `CommandBatchWorkload` which work together to create the command family workload


### **Testing:**
1. Start two splinter nodes with the experimental feature "back-pressure"
2. Create a circuit between the nodes, ensure that the scabbard version is set to 2 when creating the circuit
3. Use scabbard CLI to upload the command smart contract
4. Use the transact CLI to start a command workload, for example:
```
transact workload --targets http://localhost:8085/scabbard/<circuit-id>/<service-id> \
--key <private-key-path> \
--target-rate 5 \
--update 2 \
--workload command \
--seed 10 \
-vv
```
Observe splinterd logs to see command family transactions being executed
Note: Because one of the possible commands is `return_invalid` occasionally the logs will show:
```
T["StaticExecutionAdapter"] INFO [sawtooth_sabre::wasm_executor::wasm_externals] InvalidTransaction: 'return_invalid' command mock error message
...
T["consensus-gsAA"] ERROR [splinter::consensus::two_phase::v2] Error while creating proposal: proposal manager error occurred: scabbard state error: transaction failed: "Wasm contract returned invalid transaction: command, 1.0"
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 23:08:54 +0000 UTC
    </div>
</div>

