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
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/363" class=".btn">#363</a>
            </td>
            <td>
                <b>
                    Idemix Update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

This PR update the Idemix dependency to its latest version that is used by the Fabric Token SDK too.
Now, the SignerConfig struct also exports the RevocationHandle that is used by the Fabric Token SDK for audit purpose.
The way the revocation handle is encoded has changed to align to what the Idemix library expects.
The unit-tests have been updated.

#### Release Note

The changes to the encoding of the revocation handle should impact anyway given that Fabric is not currently using it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-29 15:00:22 +0000 UTC
    </div>
</div>

