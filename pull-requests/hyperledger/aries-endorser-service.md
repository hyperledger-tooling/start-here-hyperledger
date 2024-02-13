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

