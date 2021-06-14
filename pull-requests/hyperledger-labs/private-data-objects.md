---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/323" class=".btn">#323</a>
            </td>
            <td>
                <b>
                    Make elliptic curve parameterizable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows to define the elliptic curve used by the PDO crypto via the
-DPDO_USE_ECDSA_CURVE flag during compile time. When not defined, the
default curve is secp256k1 as used in BTC. This commit is motivated by
the use of the PDO crypto with Fabric Private Chaincode. In Fabric,
however, the default ellipctic curve is secp256r1 (aka prime256v1). This
compile flag allows to change the curve when used with FPC to be
complient with Fabric.

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 13:45:20 +0000 UTC
    </div>
</div>

