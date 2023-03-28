---
layout: default
title: firefly-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-samples
---

# firefly-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-samples/pull/52" class=".btn">#52</a>
            </td>
            <td>
                <b>
                    Initial UI & CLI token-minting sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds 2 minting samples, a UI and CLI, which are designed to be used together.

The UI sample shows the current balance of a pre-defined token pool name (`MINTSAMPLE`) and lets you mint new tokens by entering a number to mint and hitting Submit.

The CLI creates an ephemeral web socket subscription for FireFly events and prints out the details of `token_transfer_confirmed` events and `blockchain_event_received` events. The former lets us conveniently show the user how many tokens were transferred. The latter let's us show them the blockchain-specific information like block number and transaction hash so they can see the transaction on a block explorer (if using FF in gateway mode).

The samples require that the user has created a FireFly stack, which by default could be a 1 member local stack but optionally could be a stack in gateway mode to a testnet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-27 08:49:40 +0000 UTC
    </div>
</div>

