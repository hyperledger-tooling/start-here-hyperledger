---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1176" class=".btn">#1176</a>
            </td>
            <td>
                <b>
                    add extra arguments to lifecycle commands for more flexibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                for instance:

```bash
APPROVE_EXTRA_ARGS="--init-required" COMMIT_EXTRA_ARGS="--init-required" ./network chaincode deploy mychaincode ../mychaincode
INVOKE_EXTRA_ARGS="--isInit" ./network chaincode invoke mychaincode '{"Args":["init"]}'
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-03 17:00:28 +0000 UTC
    </div>
</div>

