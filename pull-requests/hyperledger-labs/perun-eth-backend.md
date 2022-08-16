---
layout: default
title: perun-eth-backend
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-eth-backend
---

# perun-eth-backend <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-eth-backend){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-eth-backend/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    Use auth.From for getting the Nonce in NewTransactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows clients to let other clients with a different account to send transactions to the adjudicator for them because now it will fetch the nonce from the address returned by the transactor which is in control of the client.
This is especially useful in the case of multi-ledger channels where a client might not be able to send transactions on a different chain s.t. a hub undertakes these transactions for the client.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 14:16:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-eth-backend/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    Fix multi ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes a few problems with the multi-ledger funder and adjudicator. See commits messages for more details.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 17:05:54 +0000 UTC
    </div>
</div>

