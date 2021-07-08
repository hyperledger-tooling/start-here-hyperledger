---
layout: default
title: perun-node
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/perun-node
---

# perun-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v0.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.6.0
                </span>
            </td>
            <td>
                perun-node v0.6.0 is a regular development release. 

Newly added:

1. Implemented a new app with text based UI (TUI) for trying out perun-node.
2. Validate contracts during node initialization.
3. Added an example for directly using the payment API by importing `perun-node` module.
    See [`app/payment/payment_test.go`](https://github.com/hyperledger-labs/perun-node/blob/master/app/payment/payment_test.go).
4. Updated the payment API to allow use of ERC20 token as currency.
    - A channel can be opened with balances in more than one currencies.
    - Multiple payments involving different currencies can be made in a single API call.
    - Asset contracts for ERC20 tokens can be specified in node config file or registered via API.

Improvements:

1. Improved error handling. The errors returned by API provide a rich context and necessary data in structured format for easy error handling.
2. Use structured logging. Request and response (success or error) are logged in a structured format for each API call.
3. Use weak (scrypt) encryption parameters for ethereum keystore wallets by default. This makes the `open session` action in tests and in CLI/TUI apps to be much faster.

For detail information on changes covered in the release, see the milestone [12](https://github.com/direct-state-transfer/dst-go/milestone/12).
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/perun-node/releases/tag/v0.6.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-07-08 09:09:20 +0000 UTC
    </span>
</div>

