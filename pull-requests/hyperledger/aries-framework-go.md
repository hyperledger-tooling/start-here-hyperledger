---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3436" class=".btn">#3436</a>
            </td>
            <td>
                <b>
                    refactor: Minimize interfaces required by didsignjwt.SignJWT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Minimized the interfaces required by the didsignjwt.SignJWT method by replacing the usage of the kms.KeyManager, crypto.Crypto, and vdr.Registry interfaces with minimized interfaces that define only the functionality needed for the SignJWT function. This makes it easier for consumers to inject in their own implementations. The method signatures of the new minimized interfaces still line up with the method signatures of the kms.KeyManager, crypto.Crypto, and vdr.Registry interfaces, so implementations of those interfaces can still be used without making any changes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-29 02:42:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3435" class=".btn">#3435</a>
            </td>
            <td>
                <b>
                    feat: wallet VerifyJWT API to verify compact jwt using DID.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 16:53:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3434" class=".btn">#3434</a>
            </td>
            <td>
                <b>
                    feat: command controller for wallet.SignJWT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-25 15:57:18 +0000 UTC
    </div>
</div>

