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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2290" class=".btn">#2290</a>
            </td>
            <td>
                <b>
                    1.0.0-rc3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR to enable creating a 1.0.0-rc3 release that matches ACA-Py Release 0.8.2.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 21:02:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2288" class=".btn">#2288</a>
            </td>
            <td>
                <b>
                    Fix routing in set public did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Having a multitenancy mode and a base wallet mediator, when a DID was being promoted to public the base wallet mediator was not taken into consideration - the returned mediation record was always None. As a result, the agent's endpoint is written to ledger instead of the mediator's.

This PR fixes this issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 09:50:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2287" class=".btn">#2287</a>
            </td>
            <td>
                <b>
                    Webhook over websocket clarification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Supersedes #2220. Thank you for your contributions @miroslav-inc!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 13:51:22 +0000 UTC
    </div>
</div>

