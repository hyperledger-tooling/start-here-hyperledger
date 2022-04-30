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
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/2" class=".btn">#2</a>
            </td>
            <td>
                <b>
                    Initial contribution from Kaleido
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See the README.md in the change for information.

Leaving in draft for now as there are some additional parts of the initial contribution pending:
- [x] README detailing references / credits
- [x] secp256k1 cryptography wrapper (ISC License)
- [x] Keystore V3 implementation (Scrypt + pbkdf2 derived keys, with AES/128/CTR encryption)
- [x] RLP encoding / decoding
- [x] Ethereum Transaction Encoding/Signing
    - [x] Original
    - [x] EIP-155
    - [x] EIP-1559 
- [x] Contribution of an existing JSON/RPC server framework for `eth_sendTransaction` based signing
    - [x] Configuration and logging in FireFly Microservice framework
    - [x] HTTPS JSON/RPC server
    - [x] `eth_sendTransaction` intercept
    - [x]  Simple `eth_getTransactionCount` support for missing Nonce
    - [x] Address lookup to Keystore V3 file
    - [x] Batch JSON/RPC support

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 14:56:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/1" class=".btn">#1</a>
            </td>
            <td>
                <b>
                    Add settings file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 14:22:21 +0000 UTC
    </div>
</div>

