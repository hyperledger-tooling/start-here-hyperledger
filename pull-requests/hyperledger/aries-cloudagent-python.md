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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1521" class=".btn">#1521</a>
            </td>
            <td>
                <b>
                    Delete unused ConnRecord generated - OOB invitation  `(use_exising_connection)`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>
- resolve #1511 
- The problem it solves:
  - If 2 agents [`Alice and Bob`] have an active connection setup (using an OOB public DID invitation)
  - `Alice` send another OOB invitation (public) to `Bob`
  - `Bob` accepts it with `use_existing_connection` option, then on `Alice` side, the invitation and associated connection generated remain unused.
- ~~This PR implements `flush_stale_connections` function, which deletes all `ConnRecords` with `state: invitation` and `invitation_mode: once` which were last updated `at least 3 hours` back. The trigger for this function is creating an OOB invitation, so whenever a new `OOB invitation` is created then this cleanup is performed. Does this strategy sound reasonable?~~
- Following feedback from @swcurran, fixed initial flawed implementation of `reuse` message and used it to accomplish deletion of `hanging` connections.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 17:00:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1519" class=".btn">#1519</a>
            </td>
            <td>
                <b>
                    added logging documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added markdown documentation of logging in Acapy.

- [x] Command Line Arguments
- [x] Environment Variables
- [x] Acapy Config
- [x] Logging Config File
- [x] Link in dev readme
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 07:53:17 +0000 UTC
    </div>
</div>

