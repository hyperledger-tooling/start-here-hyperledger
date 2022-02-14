---
layout: default
title: fabric-chaincode-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-java
---

# fabric-chaincode-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/226" class=".btn">#226</a>
            </td>
            <td>
                <b>
                    Fix transaction serializer usage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes the issue of having a single transaction serializer in use for
all contracts regardless of configuration. The issue was due to
having a singleton instance of ExecutionService that had only one
associated serializer. Thus, the first used serializer was also used
for all other transactions. The fix removes this singleton and replaces
it with a ContractRouter field.

#225

Signed-off-by: Bogdan Repeta <github@foglie.33mail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-13 22:12:40 +0000 UTC
    </div>
</div>

