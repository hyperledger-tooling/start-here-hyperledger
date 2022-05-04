---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1328" class=".btn">#1328</a>
            </td>
            <td>
                <b>
                    Ensure that connector errors finishes caliper transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A Scenario was discovered where if you send a single txn and the
connector throws an error then that single txn never finishes and the
worker loops forever waiting for that transaction to finish.

eg in the workload

```
invokerIdentity: 'unknownuser'
```

example benchmark
```
test:
  name: fixed-asset-test
  description: >-
    This is a test yaml for the existing fixed-asset benchmarks
  workers:
    type: local
    number: 1
  rounds:
    - label: empty-contract-evaluate
      chaincodeID: fixed-asset
      txNumber: 1
      rateControl:
        type: fixed-rate
        opts:
          tps: 2
      workload:
        module: benchmarks/api/fabric/workloads/empty-contract.js
        arguments:
          chaincodeID: fixed-asset
          consensus: false
```

In the wider support for connectors though the caliper framework should
ensure that connectors that either don't handle errors or throw errors
should make sure that the submission is registered as a failure (which
is what a connector would do if it did catch an error)

This fix ensures that any error received will mark a transaction as
finished

closes #1068

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 08:43:37 +0000 UTC
    </div>
</div>

