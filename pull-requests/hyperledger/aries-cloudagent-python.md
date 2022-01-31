---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1616" class=".btn">#1616</a>
            </td>
            <td>
                <b>
                    PR for endorser support to update endpoints on ledger.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a PR that contains logic which would enable the endpoint to get updated on ledger after the endorser has signed the transaction.

The endpoints that have undergone changes are : 
1.) /wallet/set-did-endpoint
2.) /wallet/did/public

These are in the /aries_cloudagent/wallet/routes.py file.

After the endpoint is updated on the ledger, it also gets updated in the wallet. The call to update it in the wallet is not included in this code, but would be implemented soon.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 16:18:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1615" class=".btn">#1615</a>
            </td>
            <td>
                <b>
                    style: format with stable black release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Black released their first stable version on January 29, resulting in the github action now failing on changes unrelated to submitted PRs. This should fix it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 13:42:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1614" class=".btn">#1614</a>
            </td>
            <td>
                <b>
                    feat: enable webhook events for mediation records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds mediation webhook topic so webhook events are sent for mediation events.

Fixes #950

@dbluhm anything I'm missing here? The change seems so trivial that I may be forgetting something
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 13:22:49 +0000 UTC
    </div>
</div>

