---
layout: default
title: firefly-signer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-signer
---

# firefly-signer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-signer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Add Signer interface to support multiple Signers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In addition to the existing secp256k1 local signer,
we can allow any provider/api that has signature generation capability
to implement the Signer interface and use firefly-signer's transaction
signing

Signed-off-by: Vinod Damle <vinod.damle@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 22:09:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Add features for performing recover for signature verification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allows for the various types of transaction (origin, EIP-155, EIP-1559) the hash payload, and transaction hash, to be calculated independently of performing signing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 20:36:43 +0000 UTC
    </div>
</div>

