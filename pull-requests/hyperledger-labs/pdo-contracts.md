---
layout: default
title: pdo-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pdo-contracts
---

# pdo-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pdo-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Add multi-issuer support for wallets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements a multi-issuer wallet. That is, a wallet that can manage (and perform operations on) assets from multiple issuers.  The wallet implements several widgets that can be used to import new issuers, check on the balance of holdings at multiple issuers (each with a unique identity), and transfer assets to other holdings (including identities with only a public key available, meaning other users running in other isolated containers).

The PR documents (or updates) three different test scenarios for the wallet:
* 06.single_user_wallet -- simple single issuer test
* 07.multiple_issuer_wallet -- test with a single wallet including multiple issuers
* 08.multier_user_wallet -- test with multiple wallets each with multiple issuers

Note that this PR does not include explicit contract flush at this point in time. That means that when refreshing the balance, it may require up to 30 seconds for the contract state to flush and be refreshed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 22:52:51 +0000 UTC
    </div>
</div>

