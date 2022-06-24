---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    Idemix MSP Folder Structure incompatible with what Fabric expects #303
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>

#### Type of change

- Bug fix

#### Description

Currently, Fabric-CA generates an Idemix MSP folder structure and file content that Fabric is not able to load.
Namely:
- The content of `SignerConfig` is encoded in json, Fabric expected proto
- Fabric expects the revocation public key to be stored in a file named `RevocationPublicKey` and `IdemixRevocationPublicKey`.

#### Additional details


#### Related issues

https://github.com/hyperledger/fabric-ca/issues/303
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 07:30:24 +0000 UTC
    </div>
</div>

