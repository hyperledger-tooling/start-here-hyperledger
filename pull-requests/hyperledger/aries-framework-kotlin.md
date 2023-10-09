---
layout: default
title: aries-framework-kotlin
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-kotlin
---

# aries-framework-kotlin <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-kotlin){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-kotlin/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Fixed pickup for queued messages. Added handling of basic messages.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes implicit pickup of queued messages from a mediator. It also adds support for basic messages which can aid in debugging as one can simply send them through the ACA-Py API.

It has been tested against a mediator running 0.4.x of ACA-Py and also against the Indicio Public Mediator. In both cases, earlier (before this PR) queued messages would not get picked up.

Now, they are correctly picked up.

Please see the following PR for work done in fixing ACA-Py routing which was also broken:
https://github.com/hyperledger/aries-cloudagent-python/pull/2536

With the above PR, and this PR, I have tested the mediator and also tested queued message delivery to this agent.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 05:21:46 +0000 UTC
    </div>
</div>

