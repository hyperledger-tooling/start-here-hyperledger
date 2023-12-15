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
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    Extend lifecycle protos to query all approved chaincode definitions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch extends lifecycle protos to query all approved chaincode definitions.

See https://github.com/hyperledger/fabric/issues/4564 for the detail.

#### Type of change

- New feature

#### Description

As a sub-task stemming from issue #4564, this patch extends lifecycle protos to query all approved chaincode definitions.
I have already done the provisional implementation and will submit them to the Fabric repository once this patch is merged.

The example of output when executing the enhanced queryapproved in the provisional implementation:

```
$ peer lifecycle chaincode queryapproved -C mychannel
Approved chaincode definition on channel 'mychannel':
name: basic2, sequence: 2, version: 1.0.1, init-required: false, package-id: basic2_1.0.1:dae4dca432d56265e87e6416b602b40e94e7f7cdc177031abda1c81d9ed4258a, endorsement plugin: escc, validation plugin: vscc
name: basic, sequence: 1, version: 1.0.1, init-required: false, package-id: basic_1.0.1:f4babb5fd92c0ab4bce8c6ac30ca7bbb4a55e6c37774582d11639b6036ae0273, endorsement plugin: escc, validation plugin: vscc
name: basic2, sequence: 1, version: 1.0.1, init-required: false, package-id: basic2_1.0.1:dae4dca432d56265e87e6416b602b40e94e7f7cdc177031abda1c81d9ed4258a, endorsement plugin: escc, validation plugin: vscc
```

```
 $ peer lifecycle chaincode queryapproved -C mychannel -O json
{
        "approved_chaincode_definitions": [
                {
                        "name": "basic2",
                        "sequence": 2,
                        "version": "1.0.1",
                        "endorsement_plugin": "escc",
                        "validation_plugin": "vscc",
                        "validation_parameter": "EiAvQ2hhbm5lbC9BcHBsaWNhdGlvbi9FbmRvcnNlbWVudA==",
                        "collections": {},
                        "source": {
                                "Type": {
                                        "LocalPackage": {
                                                "package_id": "basic2_1.0.1:dae4dca432d56265e87e6416b602b40e94e7f7cdc177031abda1c81d9ed4258a"
                                        }
                                }
                        }
                },
                {
                        "name": "basic",
                        "sequence": 1,
                        "version": "1.0.1",
                        "endorsement_plugin": "escc",
                        "validation_plugin": "vscc",
                        "validation_parameter": "EiAvQ2hhbm5lbC9BcHBsaWNhdGlvbi9FbmRvcnNlbWVudA==",
                        "collections": {},
                        "source": {
                                "Type": {
                                        "LocalPackage": {
                                                "package_id": "basic_1.0.1:f4babb5fd92c0ab4bce8c6ac30ca7bbb4a55e6c37774582d11639b6036ae0273"
                                        }
                                }
                        }
                },
                {
                        "name": "basic2",
                        "sequence": 1,
                        "version": "1.0.1",
                        "endorsement_plugin": "escc",
                        "validation_plugin": "vscc",
                        "validation_parameter": "EiAvQ2hhbm5lbC9BcHBsaWNhdGlvbi9FbmRvcnNlbWVudA==",
                        "collections": {},
                        "source": {
                                "Type": {
                                        "LocalPackage": {
                                                "package_id": "basic2_1.0.1:dae4dca432d56265e87e6416b602b40e94e7f7cdc177031abda1c81d9ed4258a"
                                        }
                                }
                        }
                }
        ]
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 11:41:26 +0000 UTC
    </div>
</div>

