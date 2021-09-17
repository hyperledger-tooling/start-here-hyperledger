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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1413" class=".btn">#1413</a>
            </td>
            <td>
                <b>
                     Make mediation invitation parameter idempotent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To ease Aca-py's deployment in scenarios where command line arguments
cannot be changed easily, make `--mediator-invitation` and
`--mediator-connections-invite` available to the `provision` command.

`provision` stores the mediator invite to be used by the agent (effectively "provisioning" it).
`start` uses the stored invite. Once used, it does not establish connection again.
If the invitation changes, the  stored value is replaced by the new one, the default mediator is cleared and the new invitation
is used to establish connection.

Boy-scouting: I split the mediation invite tests apart from the other ones for the sake of easier comprehension/code management.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 13:37:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1411" class=".btn">#1411</a>
            </td>
            <td>
                <b>
                    Make requested attributes and predicates required on indy proof request
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
        Created At 2021-09-13 16:25:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1409" class=".btn">#1409</a>
            </td>
            <td>
                <b>
                    Log warning when unsupported problem report code is received
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1397 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 21:36:50 +0000 UTC
    </div>
</div>

