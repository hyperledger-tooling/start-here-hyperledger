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
                PR <a href="https://github.com/hyperledger/transact/pull/130" class=".btn">#130</a>
            </td>
            <td>
                <b>
                    Update workload to handle TooManyRequests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates workload to handle the TooManyRequests response from a target by sleeping and attempting to submit the same batch until successful.

Running the `transact workload` command with -vv will print a message in the logs stating that the batch is being resubmitted when a `TooManyRequests`  message is received from the target 

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
--workload smallbank \
-vv
```
The log messages should look something like this
```
Smallbank-Workload-0: May-11-2021 21:42:38.758, Sent: 10, Queue Full 0, Batches/s 4.914
Smallbank-Workload-0: May-11-2021 21:42:40.838, Sent: 9, Queue Full 0, Batches/s 4.326
Smallbank-Workload-0: May-11-2021 21:42:43.123, Sent: 10, Queue Full 0, Batches/s 4.377
Smallbank-Workload-0: May-11-2021 21:42:45.168, Sent: 9, Queue Full 0, Batches/s 4.402
Received TooManyRequests message from target, attempting to resubmit batch
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 18:59:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/129" class=".btn">#129</a>
            </td>
            <td>
                <b>
                    Fix manual implementation of Option::map lint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes a lint introduced in the 1.52.0 release of Rust
flagging items like

    match Some(0) {
        Some(x) => Some(x + 1),
        None => None,
    };

Use instead:

    Some(0).map(|x| x + 1);

In some cases this requires an `as &(dyn Error + 'static)`

See for
    https://rust-lang.github.io/rust-clippy/master/index.html#manual_map
for details

Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 15:46:08 +0000 UTC
    </div>
</div>

