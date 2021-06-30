---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    fixes for new connection_protocol field in messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

Fixes to support the new connection_protocol field. This will fix all failing tests across AIP20 and AIP10, except for one JSON_LD test, which I believe is expected to fail.  This PR has to be merged with #1281 in aries-cloudagent-python to work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 01:12:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/269" class=".btn">#269</a>
            </td>
            <td>
                <b>
                    Add dockers to docker network to fix ngrok issues for mobile
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
        Created At 2021-06-29 16:43:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    fix typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

conection instead of connection. :(
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 19:23:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/266" class=".btn">#266</a>
            </td>
            <td>
                <b>
                    Cred id bypass invite create
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the secondary get of the inviter's connection_id at the point the invitee accepts the invitation in the 160 Connection Protocol tests. There is now a call to get the connection id based on the invitation id. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 19:47:43 +0000 UTC
    </div>
</div>

