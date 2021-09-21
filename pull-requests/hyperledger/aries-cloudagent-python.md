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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1420" class=".btn">#1420</a>
            </td>
            <td>
                <b>
                    When fetching the admin config, don't overwrite webhook settings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 22:23:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1416" class=".btn">#1416</a>
            </td>
            <td>
                <b>
                    unprotect liveness and readiness endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently liveness and readiness endpoints are protected by api key, it's difficult to provide agent status to external probs without revealing the key in clear text. Suggest to make the two endpoints unprotected.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 04:12:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1415" class=".btn">#1415</a>
            </td>
            <td>
                <b>
                    Fix issue with startup sequence for faber agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                for `... --multitenant --cred-type json-ld` need to start the agent before creating a DID

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 21:11:02 +0000 UTC
    </div>
</div>

