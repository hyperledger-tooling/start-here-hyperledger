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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2077" class=".btn">#2077</a>
            </td>
            <td>
                <b>
                    Issue #2068 boolean flag change
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
        Created At 2023-01-13 22:47:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2076" class=".btn">#2076</a>
            </td>
            <td>
                <b>
                    Docker images and GHA for publishing images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">help wanted</span>
            </td>
            <td>
                This PR is a reopening of #1888 and still contains some of the issues discussed on that PR. If someone wants to tackle some of those issues (whether actually using this branch or just taking inspiration -- either way is fine with me!), I'd be happy to see this fixed up and working.

cc @WadeBarnes @swcurran 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 15:55:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2075" class=".btn">#2075</a>
            </td>
            <td>
                <b>
                    WIP fix multitenant/mediation in demo, now getting aca-py error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Tweaked the mediation code in the alice/faber demo (wasn't working properly) and am now getting an error when in multitenant mode.

Each tenant agent (sub-wallet) connects to the mediator and requests mediation.  When trying to send the mediation request a "connection not found" error is raised.  I believe this is because at some point the code is falling back to "base wallet" mode and not finding the mediator connection (which is in the sub-wallet).

If you checkout my branch, start up a local von-network and then run:

`./run_demo faber --aip 10 --mediation --multitenant` 

... you will see the error.

(A similar error occurs with alice (receiving the invite) and also in `--aip 20` mode)

Exception below (faber agent):

```
Faber      |   File "/home/indy/aries_cloudagent/messaging/models/base_record.py", line 239, in retrieve_by_id
Faber      |     cls.RECORD_TYPE, record_id, {"forUpdate": for_update, "retrieveTags": False}
Faber      |   File "/home/indy/aries_cloudagent/storage/askar.py", line 95, in get_record
Faber      |     raise StorageNotFoundError(f"Record not found: {record_type}/{record_id}")
Faber      | aries_cloudagent.storage.error.StorageNotFoundError: Record not found: connection/a5429de3-d4e7-4980-a905-6ee8f00478ad
Faber      | 2023-01-10 19:39:01,180 aries_cloudagent.admin.server ERROR Handler error with exception: Record not found: connection/a5429de3-d4e7-4980-a905-6ee8f00478ad.
Faber      | Traceback (most recent call last):
Faber      |   File "/home/indy/aries_cloudagent/protocols/connections/v1_0/routes.py", line 537, in connections_create_invitation
Faber      |     mediation_id=mediation_id,
Faber      |   File "/home/indy/aries_cloudagent/protocols/connections/v1_0/manager.py", line 211, in create_invitation
Faber      |     self.profile, connection, mediation_record
Faber      |   File "/home/indy/aries_cloudagent/protocols/coordinate_mediation/v1_0/route_manager.py", line 195, in route_invitation
Faber      |     skip_if_exists=True,
Faber      |   File "/home/indy/aries_cloudagent/multitenant/route_manager.py", line 87, in _route_for_key
Faber      |     keylist_updates, connection_id=mediation_record.connection_id
Faber      |   File "/home/indy/aries_cloudagent/messaging/responder.py", line 82, in send
Faber      |     return await self.send_outbound(outbound)
Faber      |   File "/home/indy/aries_cloudagent/admin/server.py", line 137, in send_outbound
Faber      |     return await self._send(profile, message)
Faber      |   File "/home/indy/aries_cloudagent/core/conductor.py", line 601, in outbound_message_router
Faber      |     profile=profile, outbound=outbound, inbound=inbound
Faber      |   File "/home/indy/aries_cloudagent/core/conductor.py", line 628, in _outbound_message_router
Faber      |     return await self.queue_outbound(profile, outbound, inbound)
Faber      |   File "/home/indy/aries_cloudagent/core/conductor.py", line 662, in queue_outbound
Faber      |     connection_id=outbound.connection_id
Faber      |   File "/home/indy/.pyenv/versions/3.6.13/lib/python3.6/asyncio/tasks.py", line 250, in _wakeup
Faber      |     future.result()
Faber      |   File "/home/indy/.pyenv/versions/3.6.13/lib/python3.6/asyncio/tasks.py", line 180, in _step
Faber      |     result = coro.send(None)
Faber      |   File "/home/indy/aries_cloudagent/protocols/connections/v1_0/manager.py", line 1077, in get_connection_targets
Faber      |     session, connection_id
Faber      |   File "/home/indy/aries_cloudagent/messaging/models/base_record.py", line 239, in retrieve_by_id
Faber      |     cls.RECORD_TYPE, record_id, {"forUpdate": for_update, "retrieveTags": False}
Faber      |   File "/home/indy/aries_cloudagent/storage/askar.py", line 95, in get_record
Faber      |     raise StorageNotFoundError(f"Record not found: {record_type}/{record_id}")
Faber      | aries_cloudagent.storage.error.StorageNotFoundError: Record not found: connection/a5429de3-d4e7-4980-a905-6ee8f00478ad
```

I've confirmed that the `connection_id` is valid for the sub-wallet.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 19:51:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2071" class=".btn">#2071</a>
            </td>
            <td>
                <b>
                    Improved validation of record attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We ran into the issue that our generated client would throw an exception whenever a CredExRecord was deleted. The reason was the record's state parameter being set to "deleted" - a value which is not in the set of allowed values as per the swagger definition.

Changes:
- `STATE_DELETED` attribute added to BaseRecord
- added a function which lists the values of all attributes that start with a common prefix (e.g. `"STATE_"`), optionally including inherited attributes. The resulting list can be used for validation.

I took the occasion to clean up validation a bit (conn-, cred_ex- and pres_ex_records) and add it where it was missing (OobRecord).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 13:50:48 +0000 UTC
    </div>
</div>

