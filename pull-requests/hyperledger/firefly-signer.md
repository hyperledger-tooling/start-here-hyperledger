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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    Add function to get ABI constructor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently, constructors do not show up in the `Functions()` getter. This adds a public function to get the constructor from an ABI, which is needed by EVM connect for contract deployment.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 18:24:11 +0000 UTC
    </div>
</div>

