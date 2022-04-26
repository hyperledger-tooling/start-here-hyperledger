---
layout: default
title: aries-mediator-service
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mediator-service
---

# aries-mediator-service <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mediator-service){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    Feature/ssl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The goal of this commit is to make it easier for other's to use the mediator in a production environment. I created two override files, one that is used for development with ngrok, and one that is a standalone configuration. The standalone configuration includes .env variables to specify the URL.

There is also a bug fix included here to fix the web sockets upgrade being case sensitive. Some client libraries will use a lower case value.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 22:17:24 +0000 UTC
    </div>
</div>

