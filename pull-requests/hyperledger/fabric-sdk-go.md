---
layout: default
title: fabric-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-go
---

# fabric-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/230" class=".btn">#230</a>
            </td>
            <td>
                <b>
                    wallets with custom walletstores as backends
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As the Wallet struct's store field is unexported it cannot be set outside the gateway package. This pull request adds a simple function to make it possible to have a custom WalletStore's.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-13 10:05:08 +0000 UTC
    </div>
</div>

