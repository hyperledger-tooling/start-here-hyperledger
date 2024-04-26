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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2919" class=".btn">#2919</a>
            </td>
            <td>
                <b>
                    :arrow_up: Upgrade pydid (pydantic v2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Testing pydid upgrade to pydantic v2: https://github.com/Indicio-tech/pydid/pull/72

Signed-off-by: ff137 <ff137@proton.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-26 11:35:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2918" class=".btn">#2918</a>
            </td>
            <td>
                <b>
                    fix: fixes a regression that requires a log file in multi-tenant mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a regression introduced by #2870 that required a log file to be present on file when using the default config setup for multi-tenant mode. The log file is only required if the user specifically sets the `--log-file` startup param.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 23:44:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2917" class=".btn">#2917</a>
            </td>
            <td>
                <b>
                    Update AnonCreds to 0.2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 13:40:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2916" class=".btn">#2916</a>
            </td>
            <td>
                <b>
                    fix: rev notifications on publish pending
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2915.

Ensure revocation notifications are emitted when publishing batched pending revocations when _not_ using an external endorser to publish the transaction.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 01:47:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2912" class=".btn">#2912</a>
            </td>
            <td>
                <b>
                    0.12.1rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 18:09:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2910" class=".btn">#2910</a>
            </td>
            <td>
                <b>
                    :bug: Fix ServiceDecorator parsing in oob record handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes `find_oob_target_for_outbound_message` and `find_oob_record_for_inbound_message` in OobMessageProcessor

Context:
Attempting to upgrade to 0.12 in https://github.com/didx-xyz/aries-cloudapi-python

Our existing OOB test workflows would raise an error from the following line in `find_oob_record_for_inbound_message`:
```py
        their_service = (
            cast(
                ServiceDecorator,
                ServiceDecorator.deserialize(oob_record.their_service),
            )
            if oob_record.their_service
            else None
        )
```

The error:
```py
Traceback (most recent call last):
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/messaging/models/base.py", line 196, in deserialize
    schema.loads(obj) if isinstance(obj, str) else schema.load(obj),
  File "/home/aries/.local/lib/python3.9/site-packages/marshmallow/schema.py", line 723, in load
    return self._do_load(
  File "/home/aries/.local/lib/python3.9/site-packages/marshmallow/schema.py", line 910, in _do_load
    raise exc
marshmallow.exceptions.ValidationError: {'_schema': ['Invalid input type.']
```

I noticed that according to the compiler, `oob_record.their_service` was already of type ServiceDecorator ... so `cast(ServiceDecorator, ServiceDecorator.deserialize(...` is especially code-smelly!

Resolving that to simply be `their_service = oob_record.their_service` led to the following exception:

```py
...
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/admin/server.py", line 148, in send_outbound
    return await self._send(profile, message)
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/core/conductor.py", line 647, in outbound_message_router
    status: OutboundSendStatus = await self._outbound_message_router(
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/core/conductor.py", line 674, in _outbound_message_router
    return await self.queue_outbound(profile, outbound, inbound)
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/core/conductor.py", line 722, in queue_outbound
    outbound.target = await self.dispatcher.run_task(
  File "/usr/local/lib/python3.9/asyncio/futures.py", line 284, in __await__
    yield self  # This tells Task to wait for completion.
  File "/usr/local/lib/python3.9/asyncio/tasks.py", line 328, in __wakeup
    future.result()
  File "/usr/local/lib/python3.9/asyncio/futures.py", line 201, in result
    raise self._exception
  File "/usr/local/lib/python3.9/asyncio/tasks.py", line 256, in __step
    result = coro.send(None)
  File "/home/aries/.local/lib/python3.9/site-packages/aries_cloudagent/core/oob_processor.py", line 110, in find_oob_target_for_outbound_message
    outbound_message.payload = json.dumps(message)
...
TypeError: Object of type ServiceDecorator is not JSON serializable
```

The above was fixed by adding `.serialize()` to `message["~service"] = oob_record.our_service.serialize()` 
Tada! With this modification, our previous OOB test workflow is passing again.

This appears to come from some type inconsistencies ... where services are references as either dictionaries or ServiceDecorator types.

Some tests were failing due to mocking their/our_service as dictionaries. Resolved that by using the correct model.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 20:46:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2909" class=".btn">#2909</a>
            </td>
            <td>
                <b>
                    Fix api schema mixup in revocation routes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/aries-cloudagent-python/issues/2901.

I somehow mixed up the schema naming between anoncreds revocation and existing revocation modules in a couple places. Shouldn't cause problems but still needs to be fixed.

Also a couple schemas existed in anoncreds that weren't used (copy and paste error)

##### ***Note***: 
This does remind me of something. The clear pending revocations method doesn't exist in the anoncreds implementation currently. Not sure how important that is and if it should be implemented for the upcoming 1.0.0 release ?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 17:24:49 +0000 UTC
    </div>
</div>

