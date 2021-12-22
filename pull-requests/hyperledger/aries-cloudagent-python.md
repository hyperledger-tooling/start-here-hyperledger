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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1574" class=".btn">#1574</a>
            </td>
            <td>
                <b>
                    Allow public invites for alice/faber demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Addresses https://github.com/hyperledger/aries-cloudagent-python/issues/1571

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-21 23:59:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1573" class=".btn">#1573</a>
            </td>
            <td>
                <b>
                    Updates for final Release 0.7.3
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
        Created At 2021-12-21 22:54:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1570" class=".btn">#1570</a>
            </td>
            <td>
                <b>
                    fix: use invitation key for connection query
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

Invitation key was not taken into account for get connections endpoint.

If possible, would like to get this in the upcoming 0.7.3 release :)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-21 16:30:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1569" class=".btn">#1569</a>
            </td>
            <td>
                <b>
                    Multi ledger: IndyDID resolver bug fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>
- resolve #1567 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-20 19:32:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1566" class=".btn">#1566</a>
            </td>
            <td>
                <b>
                    DiscoveryExchangeRecord RECORD_TOPIC typo fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 23:15:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1565" class=".btn">#1565</a>
            </td>
            <td>
                <b>
                    Update docker scripts to use new & improved docker IP detection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Required to support newer versions of docker

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 18:02:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1564" class=".btn">#1564</a>
            </td>
            <td>
                <b>
                    Fix the inconsistency of invitation_msg_id between invitation and response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi!
This PR fixes the inconsistency of invitation_msg_id between invitation and response when connection is reused.

### example of problem
`receive-invitation` with invitation
{"@type": "did:sov:BzCbsNYhMrjHiqZDTUASHg;spec/out-of-band/1.0/invitation", "@id": "**6ccba5e9-2b8d-4071-bd91-0058d5187d79**", "services": ["did:sov:2ACCk6nnJQmaibXp5yiXZA"], ...

The response of `receive-invitation`
{"my_did": "VrN5qwVB7ewV43C679ekUx", "invitation_msg_id": "**a7753007-5e3f-4583-826b-ae94550fed15**", "their_public_did": "2ACCk6nnJQmaibXp5yiXZA", ...

### solution
Fetch the connection record after reuse handshake.

Thanks!

Signed-off-by: Ethan Sung <baegjae@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 07:06:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1563" class=".btn">#1563</a>
            </td>
            <td>
                <b>
                    Typo vdr service name
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
        Created At 2021-12-16 21:46:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1562" class=".btn">#1562</a>
            </td>
            <td>
                <b>
                    chore: update pydid to ^0.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should have a pretty minimal impact on things while enabling resolution of Documents with nonconforming `@context` attributes (spec defines that context must be a list of strings, some docs have embedded contexts). Also solves the bug mentioned in this comment from forever ago: https://github.com/hyperledger/aries-cloudagent-python/pull/1218#issuecomment-890591874
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 20:19:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1561" class=".btn">#1561</a>
            </td>
            <td>
                <b>
                    Add alias field to didexchange invitation UI
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
        Created At 2021-12-16 17:56:30 +0000 UTC
    </div>
</div>

