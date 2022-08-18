---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/370" class=".btn">#370</a>
            </td>
            <td>
                <b>
                    Add WithEndorsersByMSPIDs to query chaincode view
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">View API</span>
            </td>
            <td>
                This adds a missing option to select the endorsing peers via MSPIDs when
performing a query. We already have this option for invoke.

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-17 10:08:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/369" class=".btn">#369</a>
            </td>
            <td>
                <b>
                    fabric-sdk: support for PKC11 #281
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                - removed bccsp section that was never used
- the default msp must be included directly under msps
- possibiilty to pass options
- PKCS11 BCCSP support and configuration

TODO:
- Option to add an identity whose secret key is stored in the HSM. Something like:
```go
borrower := fscTopology.AddNodeByName("borrower")
borrower.AddOptions(fabric.WithHSMIdentity("b1"))
```
- Extend NWO to generate the HSM identities:
  - Add an HSM flag to `PeerIdentity`
  - `integration/nwo/fabric/network/network_support.go Line 678`: Parse HSM identities from Opts and add `PeerIdentity`
  - `integration/nwo/fabric/network/network.go`: Add to `GenerateArtifacts` the generation of the HSM identities.
- Extend the `IOU` integration test to use this identity. The burrower can use this identity for the ownership of the IOU state.



Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 13:07:06 +0000 UTC
    </div>
</div>

