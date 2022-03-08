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
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/27" class=".btn">#27</a>
            </td>
            <td>
                <b>
                    Simplify the startup and upgrade the docs for nubes like me
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Being somewhat new to running an agent / mediator I struggled quite a bit getting one started. Out of this came some reworking of the project to make it ***just work*** for developers with `docker-compose up`. My though is its good enough to get running and once started it can be adapted to run on k8s, AWS, or the likes.

- Updated the docs to explain what the components are and why they're started;
- Use docker health checks to determine start conditions for dependencies;
- Only run as a docker stack; not really meant to run containers independently. This removed the need for the `manage` script.
- Removed wait-for-it subdue because startup conditions take care of this;
- Removed tunnelling and nginx in favour of a single ngrok process with caddy proxying and redirecting both ports.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-08 15:04:54 +0000 UTC
    </div>
</div>

