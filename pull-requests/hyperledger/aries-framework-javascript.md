---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/332" class=".btn">#332</a>
            </td>
            <td>
                <b>
                    mediation 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                this pr contains the needed code for mediation protocol.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 18:07:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/331" class=".btn">#331</a>
            </td>
            <td>
                <b>
                    feat: allow for lazy wallet initialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - remove agent `closeAndDeleteWallet` as it was only used for tests. They now inject the wallet to close and delete
- make `walletConfig` and `walletCredentials` optional in `InitConfig`
- user can now manually initiale the wallet
- If agent is initialized and wallet is not yet initialized and no `walletConfig` and `walletCredentials` are available an error will be thrown
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 16:32:26 +0000 UTC
    </div>
</div>

