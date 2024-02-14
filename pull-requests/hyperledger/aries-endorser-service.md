---
layout: default
title: aries-endorser-service
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-endorser-service
---

# aries-endorser-service <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-endorser-service){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    Allowance endpoints - collection name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses the minor discrepancies here https://github.com/hyperledger/aries-endorser-service/issues/41
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 00:34:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    Change docker compose to the ngrok/ngrok image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `wernight/ngrok` image is out of date and you can get Ngrok token errors with the age of the agent.

Update to the `ngrok/ngrok` that is used elsewhere in the hyperledger and aca-py ecosystems. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 23:21:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    Add ngrok setup and documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These days one needs a token to use Ngrok. Starting up the endorser service locally is failing currently with the existing instructions.

Add instructions to add your token to an `env` and import that into the ngrok container.

As a note, most of the other stuff in our ecosystem I believe uses `ngrok/ngrok` as the image whereas this one is still using `image: wernight/ngrok`. Might be a task for later to reconcile that?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 19:40:02 +0000 UTC
    </div>
</div>

