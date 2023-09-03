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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2458" class=".btn">#2458</a>
            </td>
            <td>
                <b>
                    WIP: Revocation API using anoncreds-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Still in infancy, having troubles mapping anoncreds-rs to current revocation API.
See issue #2432.

Next step is to work on the BDD tests in `0586-sign-transaction.feature`, enable those and get those working. Perhaps should have started there earlier and would have given me a more focused path forward. 🤷 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-01 22:13:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2456" class=".btn">#2456</a>
            </td>
            <td>
                <b>
                    Update Python image version to 3.9.18
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Reduces the number of vulnerabilities in the image.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 12:25:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2454" class=".btn">#2454</a>
            </td>
            <td>
                <b>
                    0.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 15:16:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2452" class=".btn">#2452</a>
            </td>
            <td>
                <b>
                    0.10.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 12:44:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2451" class=".btn">#2451</a>
            </td>
            <td>
                <b>
                    chore: relax connections filter DID format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Relax the connection filter on `my_did`, `their_did` and `their_public_did` fields of the `/connections` endpoints.

These values were restricted to `did:sov` and are now open to the generic DID format.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 13:16:30 +0000 UTC
    </div>
</div>

