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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2465" class=".btn">#2465</a>
            </td>
            <td>
                <b>
                    chore: add black back in as a dev dep
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I'm not sure what happened -- or perhaps I'm just imagining that it was in our dev deps before -- but black wasn't in our pyproject.toml so I added it back in. And associated lock update.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 00:34:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2464" class=".btn">#2464</a>
            </td>
            <td>
                <b>
                    feat: add timeout to did resolver resolve method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a `timeout` parameter to the DID Resolver interface, defaulting to 30 seconds. Without it, a poorly behaved resolver plugin can "resolve" documents that aren't actually DID Docs and cause ACA-Py to run out of memory.

There's space for additional tuning on the timeout default. Some DID Methods are, in my experience, quite slow (did:btcr and did:ion resolvers can be pretty slow sometimes). 30 seconds might be overly charitable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 00:31:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2461" class=".btn">#2461</a>
            </td>
            <td>
                <b>
                    fix: issue #2434: Change DIDExchange States to Match rfc160
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes fixes to https://github.com/hyperledger/aries-cloudagent-python/issues/2434. Changes all `ConnRecord.States` to match that of rfc160.

For additional information, here's the identical PR with some feedback from @dbluhm ~ 
https://github.com/Indicio-tech/aries-cloudagent-python/pull/151
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 18:46:54 +0000 UTC
    </div>
</div>

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

