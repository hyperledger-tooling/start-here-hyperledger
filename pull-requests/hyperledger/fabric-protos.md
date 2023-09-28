---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/190" class=".btn">#190</a>
            </td>
            <td>
                <b>
                    Extend lifecycle protos to checkcommitreadiness to provide discrepancy details
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch extends lifecycle protos to checkcommitreadiness to provide discrepancy details.

#### Type of change

- New feature

#### Description
I have proposed an extension to lifecycle chaincode checkcommitreadiness to provide details of the discrepancies as shown in  https://github.com/hyperledger/fabric/issues/4428.

As a sub-task stemming from issue #4428, this patch extends lifecycle protos to checkcommitreadiness to provide discrepancy details.
To maintain backward compatibility with the previous versions of checkcommitreadiness, I've opted to introduce a field named `mismatches`.

Once this patch is merged, I plan to enhance the command and submit it to the Fabric repository. A provisional implementation is provided below:
- https://github.com/satota2/fabric/commit/58db22d9c9d5d04f10001cb45329e2f440d0a5b3
- https://github.com/satota2/fabric/commit/9ea8ad11de451139af61cf73281feff656a38d07

The example of output when executing checkcommitreadiness with inspect flag in the provisional implementation:

```
peer lifecycle chaincode checkcommitreadiness --channelID mychannel --name basic --version 2.0 --sequence 2 --inspect
Chaincode definition for chaincode 'basic', version '2.0', sequence '2' on channel 'mychannel' approval status by org:
Org1MSP: false (mismatch: [EndorsementInfo, ValidationInfo, Collections])
Org2MSP: false (mismatch: [ChaincodeParameters])
```

```
peer lifecycle chaincode checkcommitreadiness --channelID mychannel --name basic --version 2.0 --sequence 2 --inspect --output json
{
        "approvals": {
                "Org1MSP": false,
                "Org2MSP": false
        },
        "mismatches": {
                "Org1MSP": {
                        "items": [
                                "EndorsementInfo (Check the Version, InitRequired, EndorsementPlugin)",
                                "ValidationInfo (Check the ValidationParameter, ValidationPlugin)",
                                "Collections (Check the Collections)"
                        ]
                },
                "Org2MSP": {
                        "items": [
                                "ChaincodeParameters (Check the Sequence, ChaincodeName)"
                        ]
                }
        }
}
```

#### Related Issues

- https://github.com/hyperledger/fabric/issues/4428
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 01:34:02 +0000 UTC
    </div>
</div>

