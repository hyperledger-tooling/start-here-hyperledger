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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2395" class=".btn">#2395</a>
            </td>
            <td>
                <b>
                    Multitenant check endorser_info before saving
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While testing PR #2339 I was using an instance without an endorser and encountered an error while saving the new write ledger: `UnboundLocalError: local variable 'endorser_alias' referenced before assignment`.

This checks to see if we have endorser information before we try to persist it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 18:50:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2394" class=".btn">#2394</a>
            </td>
            <td>
                <b>
                    feat: add DID Exchange specific problem reports and reject endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes problem reports sent during the DID Exchange protocol have the DID Exchange protocol adopted problem report rather than the generic problem report. This is defined in RFC 23 but has not been implemented by ACA-Py to this point. In other words, this is a correction to bring ACA-Py more in line with the RFC. These problem reports were automatically sent if there was an issue in processing the DID Exchange messages.

In addition to the above changes, this PR also introduces a `POST /didexchange/{conn-id}/reject` endpoint, enabling the controller to explicitly reject an OOB invitation that specifies DID Exchange as the handshake protocol or a DID Exchange request. Rejecting a response is not supported; don't send a request if you're going to reject the response. This will send a problem report to the originator of the invitation/request and will mark the (local) connection record as abandoned. It won't delete the record though (maybe it should)?

This at least partially supersedes #2350, covering the rejection of invitations to exchange DIDs. However, it does not introduce automatic handling of timeouts for invitations, as was discussed in the comments.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 13:27:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2393" class=".btn">#2393</a>
            </td>
            <td>
                <b>
                    fix: outbound send status missing on path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This corrects a flow through the `queue_outbound` method that could result in no `OutboundSendStatus` being returned. The method is strictly expected to return a status so this could cause less than graceful errors in some circumstances.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 11:52:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2392" class=".btn">#2392</a>
            </td>
            <td>
                <b>
                    fix: additional tweaks for did:web and other methods as public DIDs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adjusts the request schema for the set public DID endpoint to permit `GENERIC_DID`s. It seems that the work to support a generic DID in this endpoint was already done and just the request schema was missed by mistake (or perhaps it's a merge artifact :man_shrugging:).

Additionally, this PR adjusts the behavior of DID Exchange requests so that if we're using a public DID, no DID Doc attachment is included in the request. This enables us to form connections using a did:web or other DID that is resolvable without worrying about ACA-Py's DID Doc creation process not being quite up to snuff on multi-method support.

And some minor type hint corrections.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-01 19:00:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2391" class=".btn">#2391</a>
            </td>
            <td>
                <b>
                    fix: keylist update response race condition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When receiving an OOB invitation and automatically accepting by sending a DID Exchange request, it is possible to send a keylist update to the mediator and receive a response back before the connection is saved. This resulted in errors like:

```
Traceback (most recent call last):
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/protocols/coordinate_mediation/v1_0/route_manager.py", line 273, in connection_from_recipient_key
    conn = await ConnRecord.retrieve_by_tag_filter(
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/messaging/models/base_record.py", line 284, in retrieve_by_tag_filter
    raise StorageNotFoundError(
aries_cloudagent.storage.error.StorageNotFoundError: ConnRecord record not found for {'invitation_key': 'qHFoiMYB58Y25wRkFfYajhFLSUvJFZZbJStiaKL1LvW'}

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/protocols/coordinate_mediation/v1_0/handlers/keylist_update_response_handler.py", line 45, in notify_keylist_updated
    key_to_connection = {
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/protocols/coordinate_mediation/v1_0/handlers/keylist_update_response_handler.py", line 46, in <dictcomp>
    updated.recipient_key: await route_manager.connection_from_recipient_key(
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/protocols/coordinate_mediation/v1_0/route_manager.py", line 280, in connection_from_recipient_key
    conn = await ConnRecord.retrieve_by_did(session, my_did=did_info.did)
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/connections/models/conn_record.py", line 313, in retrieve_by_did
    return await cls.retrieve_by_tag_filter(session, tag_filter, post_filter)
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/messaging/models/base_record.py", line 284, in retrieve_by_tag_filter
    raise StorageNotFoundError(
aries_cloudagent.storage.error.StorageNotFoundError: ConnRecord record not found for {'my_did': '2XamEWAbXkzx4eKW24PmSY'}

The above exception was the direct cause of the following exception:

Traceback (most recent call last):
  File "/usr/local/lib/python3.9/asyncio/tasks.py", line 256, in __step
    result = coro.send(None)
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/core/dispatcher.py", line 269, in handle_message
    await handler(context, responder)
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/protocols/coordinate_mediation/v1_0/handlers/keylist_update_response_handler.py", line 31, in handle
    await self.notify_keylist_updated(
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/protocols/coordinate_mediation/v1_0/handlers/keylist_update_response_handler.py", line 52, in notify_keylist_updated
    raise HandlerException(
aries_cloudagent.messaging.base_handler.HandlerException: Unknown recipient key received in keylist update response
```

Under this condition, this makes it impossible for the keylist update response event emitter to know what connection the updated key was associated with. This PR addresses this by ensuring the DID is associated with the connection record before emitting a keylist update to the mediator.

~~There is a side effect to this change: one additional connection webhook will be emitted where the only change from the previous webhook will be a value for `my_did`; the state will not change from `invitation-received`. It's possible a controller might not like this -- though I think that would be a sign of other issues.~~ Nevermind, I solved this issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-31 22:22:10 +0000 UTC
    </div>
</div>

