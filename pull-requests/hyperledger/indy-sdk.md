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
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2505" class=".btn">#2505</a>
            </td>
            <td>
                <b>
                    allow issuance of multiple cred at same revocation index
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR proposes an option for the issuer to specify a cred_rev_id (index in revocation registry) when a credential is issued.This gives more control for an issuer to manage revocation registry, a few examples can be

- Alice issues credentials with same cred_rev_id multiple times to Bob, who wants the same credential to be stored in multiple wallets, In this case Alice can revoke a credential of Bob by revoking a single index, this allows Alice to create a better controller logic for revocation registry
- Alice issues credentials with same cred_rev_id to multiple Holders e.g. Coupons

@DaevMithran


Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-27 07:43:40 +0000 UTC
    </div>
</div>

