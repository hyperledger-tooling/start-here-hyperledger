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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2230" class=".btn">#2230</a>
            </td>
            <td>
                <b>
                    stand up multiple agents (single and multi) for local development and testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While working on load testing for [Aries Mediator Service](https://github.com/hyperledger/aries-mediator-service) I needed to spin up multiple agents and needed help to see a simple way to do so; at least not vanilla instances that I could run ad-hoc test scripts against.

I required multiple single-tenant mode and a multi-tenant mode to test our mediation between multiple agents. This was a simple way to achieve it. I decided I would stand up the standard `faber`, `alice`, `acme` single-tenant agents and one multi-tenant agent.

I did opt to include a Postgresql server shared across all the agents and included ngrok (easily turned off per agent) for URLs accessible outside the local network.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 19:46:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2229" class=".btn">#2229</a>
            </td>
            <td>
                <b>
                    Connection target should not be limited only to indy dids
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 13:00:01 +0000 UTC
    </div>
</div>

