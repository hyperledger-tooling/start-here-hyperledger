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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1530" class=".btn">#1530</a>
            </td>
            <td>
                <b>
                    Enable WS Pings for WS Inbound Transport
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When connecting over WS, it is impossible for ACA-Py to detect when the other end has unexpectedly closed (no WS close or error message sent) without using a heartbeat and timeout. With these changes, if a mobile agent connected over WS suddenly loses connectivity (wifi or data signal drops, for instance), the window of time where a message can be lost due to ACA-Py not realizing the WS has entered a bad state is shrunk to at most `timeout_interval` seconds. An image with a version of these changes has been in testing in a live mediator deployment for a couple of months now with much success.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 16:12:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1528" class=".btn">#1528</a>
            </td>
            <td>
                <b>
                    Fix integration tests (revocation notifications)
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
        Created At 2021-12-01 23:55:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1527" class=".btn">#1527</a>
            </td>
            <td>
                <b>
                    Add Revocation notification support to alice/faber
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
        Created At 2021-12-01 22:24:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1526" class=".btn">#1526</a>
            </td>
            <td>
                <b>
                    Display QR code when generating/displaying invites on startup
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
        Created At 2021-12-01 18:01:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1525" class=".btn">#1525</a>
            </td>
            <td>
                <b>
                    OOB: Fixes issues with multiple public explicit invitation and unused 0160 connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>
- resolves #1524
- Updated `ConnectionManager` and `DIDXManager` to look up `ConnRecord` by `invitation_msg_id`
- Also fixes the issue, when an OOB invitation [`0160` and with public DID] is accepted by the invitee, on the inviter side, a new `ConnRecord` is created and activated, and the original `ConnRecord` created along with the invitation remains unused.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 20:11:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1523" class=".btn">#1523</a>
            </td>
            <td>
                <b>
                    added documentation for wallet storage databases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - [x] SQlite
- [x] PostgreDB
- [x] Link in other documentation
- [x] Docker Compose example
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 09:46:44 +0000 UTC
    </div>
</div>

