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
                PR <a href="https://github.com/hyperledger/transact/pull/310" class=".btn">#310</a>
            </td>
            <td>
                <b>
                    Add sleep in `BatchStatusChecker` loop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a 0.25 second sleep to the end of the loop in the `BatchStatusChecker` thread to lower the command workload CPU usage.

Comparison test:
1. Started two splinter nodes locally, created a circuit and uploaded the command smart contract
2. Started a transact workload from the transact main branch
``` 
cargo run --manifest-path cli/Cargo.toml workload \
--target-rate 5/s \
--workload command \
-vv \
--targets 'http://localhost:28080/scabbard/<circuit_id>/<service_id>' \
```
3. Use top to check cpu% of transact - peak was around 53.8% after running the workload for 20 minutes
4. Stopped the workload and started a new workload with the change in this branch, using the same workload command as above
5. Use top to check cpu% of transact - peak was around 5.2% after running the workload for 20 minutes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 18:22:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/309" class=".btn">#309</a>
            </td>
            <td>
                <b>
                    Update sha2 dependency to 0.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This update is meant to track the latest release and
does not require any updates.

Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 20:51:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/308" class=".btn">#308</a>
            </td>
            <td>
                <b>
                    Move Hyperledger Sawtooth Sabre TransactionHandler into Transact's families
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Moves the transaction handler, protos and protocol into the Transact library. This includes retaining the Sabre commit history.

See the draft PR https://github.com/hyperledger/sawtooth-sabre/pull/171 for verification that it works, specifically the integration test.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 17:36:16 +0000 UTC
    </div>
</div>

