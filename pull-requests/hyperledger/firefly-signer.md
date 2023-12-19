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
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    Update receipts and TX info
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Having a mix of capitalization was causing some issues in a variety of ways. This change normalizes to lowercase, and then leaves it up to the calling code if it wants to display and address with a checksum or not.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 16:17:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    Offline signer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Create a simple command-line to sign and submit a transaction, without needing to run the server and make a HTTP call.

Example that works for a `ff` created example Eth network running on `http://localhost:5100`:

```sh
go run ./ffsigner/main.go send-transaction -f ./test/offline-signer.conf.yaml -i ./test/offline-tx.json
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 23:19:26 +0000 UTC
    </div>
</div>

