---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/542" class=".btn">#542</a>
            </td>
            <td>
                <b>
                    Refactor connection protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Removes forgotten `disclose` protocol handling on Aries SM level
- Weakens assumptions about connection confirmation message on Connection protocol Aries SM level. We have required that inviter must receive Ping or Ack message to progress to final state on Inviter side, however as [rfc states](https://github.com/hyperledger/aries-rfcs/blob/main/features/0160-connection-protocol/README.md#3-connection-acknowledgement), "any message will do":
> After the Response is received, the connection is technically complete. This remains unconfirmed to the inviter however. The invitee SHOULD send a message to the inviter. As any message will confirm the connection, any message will do.

So instead of having `handle_ping` and `handle_ack` in inviter SM, these are replaced by `handle_confirmation_message`. If the final message happens to be `Ping`, it's up to upper layers to perhaps respond to ping, but shouldn't be part of Connection SM responsibility to respond Ping message (and no longer is, with the changes made).
- Adds optional thread attribute to `BasicMessage`
- Adds thread_id matching for all message types. 
- Update `verify_thread_id` to not skip thread verification if `indy_mocks_enabled == true`
- Renamed `handle_connect` to more descriptive names `send_connection_request` for invitee and `create_invitation` for inviter FSMs.

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 15:28:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/541" class=".btn">#541</a>
            </td>
            <td>
                <b>
                    Reformat code with rustfmt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addressing https://github.com/hyperledger/aries-vcx/issues/540
- configured max line length to 120 chars
- added script to configure git pre-commit hook to reformat modified files
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 10:08:43 +0000 UTC
    </div>
</div>

