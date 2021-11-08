---
layout: default
title: indy-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk
---

# indy-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2440" class=".btn">#2440</a>
            </td>
            <td>
                <b>
                    fix(objective c wrapper) NSError should be nil when there is no error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: conanoc <conanoc@gmail.com>

Returning NSError with error code **Success** makes trouble sometimes.
The following code snippet opens a wallet using async/await in swift5. It always throws error and does not return wallet handle because the error included in the completion handler is not nil.
```swift
    let wallet = IndyWallet.sharedInstance()!
    var walletHandle : IndyHandle?
    do {
        walletHandle = try await wallet.open(withConfig: walletConfig, credentials: walletCredentials)
    } catch {
        if let err = error as NSError? {
            print("Cannot open wallet: \(err.userInfo["message"] ?? "Unknown error")")
        }
        return
    }
```

So, NSError should be nil when the indy_error_code is Success.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 02:48:28 +0000 UTC
    </div>
</div>

