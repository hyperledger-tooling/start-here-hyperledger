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
3. Use scabbard CLI to upload the smallbank smart contract contract
4. Use the transact CLI to start a workload, for example:
```
transact workload --targets http://splinterd-beta:8085/scabbard/<circuit-id>/<service-id> \
--key <private-key-path> \
--target-rate 5 \
--update 2 \
--workload command \
--seed 10
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/139" class=".btn">#139</a>
            </td>
            <td>
                <b>
                    Run just recipes in CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 01:05:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/138" class=".btn">#138</a>
            </td>
            <td>
                <b>
                    Move Database-backed MerkleTree to kv submodule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change moves the existing merkle tree implementation to a kv submodule and re-exports it from the original module. This provides a space for additional back-end implementations.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 21:49:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/137" class=".btn">#137</a>
            </td>
            <td>
                <b>
                    Fix Transact docker builds with Docker Compose 1.28+
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 19:11:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/136" class=".btn">#136</a>
            </td>
            <td>
                <b>
                    Change wait time between batch submit responsively
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Transact waits the full time between the end of one batch submit and the
next regardless of how long the submit takes. This can make the target
submission rate and the actual submission rate be very different.
This change alters the time between submissions based on how long the
current submission took and a "best guess" for how long they usually
take.
Ideally this will more tightly tie the target and actual submission rate.

Signed-off-by: Caleb Hill <hill@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 13:02:53 +0000 UTC
    </div>
</div>

