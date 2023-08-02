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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2365" class=".btn">#2365</a>
            </td>
            <td>
                <b>
                    Corrected typo on mediator invitation configuration argument
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
        Created At 2023-07-29 00:04:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2362" class=".btn">#2362</a>
            </td>
            <td>
                <b>
                    Fix empty ServiceDecorator in OobRecord causing 422 Unprocessable Entity Error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves  #2242
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-28 08:28:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2356" class=".btn">#2356</a>
            </td>
            <td>
                <b>
                    :rocket: Performance Boost: Replace json with orjson through JsonUtil class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The [orjson](https://github.com/ijl/orjson) library provides superior performance over the built-in json module. Please see their readme for an overview of features and performance/runtime comparisons.

One note is: `orjson.dumps` serializes to `bytes`, instead of `str`, so it's not a drop in replacement.
Edit: it also omits whitespace between keys and values. i.e. json.dumps: `{"k": [1, 2, 3]}`. orjson.dumps:  `{"k":[1,2,3]}`

There are 449 usages of `json.dumps` throughout the codebase. To refactor, I would just want to regex replace all of those with `orjson.dumps`, but then it would require appending `.decode()` as well (for bytes -> string).

That inspired me to create a JsonUtil class in `utils.json.py`. So, I could replace all instances of `json.loads` and `json.dumps` with `JsonUtil.*`.

This also has the benefit of providing an abstraction layer to simplify future transitions between different JSON libraries.

Note: I had to replace `import json` with `from aries_cloudagent.utils.json import JsonUtils`. Re-added `import json` where needed. However, that means the import organisation is no longer consistent, because json is a top-level import, and the utils import shouldn't be. Nitpick, bit I would want to do a import sort across all files to fix this ...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 17:40:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2355" class=".btn">#2355</a>
            </td>
            <td>
                <b>
                    Correct the response type in `send_rev_reg_def`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Simple fix: the `send_rev_reg_def` method can return a `rev_reg: IssuerRevRegRecord`, which doesn't line up with the expected schema (`TxnOrRevRegResultSchema`).

TLDR: 
- the OpenAPI spec says the response is a `TxnOrRevRegResultSchema`, 
- but it's actually a `Union[RevRegResult, TxnOrRevRegResult]`.

As the name suggests, the `RevRegResult` should be wrapped in a `TxnOrRevRegResult`, which this PR fixes.

Initially typed out an issue, so just to show my working:
___
In the definition for the `send_rev_reg_def` method (in [`/aries_cloudagent/revocation/routes.py`](https://github.com/hyperledger/aries-cloudagent-python/blob/8b6c87fba2a6dc6cce4ced92d4db554fb4cad37a/aries_cloudagent/revocation/routes.py#L1019)), the response schema is indicated to be a `TxnOrRevRegResultSchema`:
```py
@response_schema(TxnOrRevRegResultSchema(), 200, description="")
async def send_rev_reg_def(request: web.BaseRequest):
```
which has the definition:
```py
class TxnOrRevRegResultSchema(OpenAPISchema):
    """Result schema for credential definition send request."""

    sent = fields.Nested(
        RevRegResultSchema(),
        required=False,
        definition="Content sent",
    )
    txn = fields.Nested(
        TransactionRecordSchema(),
        required=False,
        description="Revocation registry definition transaction to endorse",
    )
```

In the [`aries-cloudcontroller-python`](https://github.com/didx-xyz/aries-cloudcontroller-python) project, we have to manually alter the model, generated from the OpenAPI spec, to correct that the response can actually be a `Union[RevRegResult, TxnOrRevRegResult]`, because that's what the server gives.

So, something is wrong with the implementation. Let's inspect [the code](https://github.com/hyperledger/aries-cloudagent-python/blob/8b6c87fba2a6dc6cce4ced92d4db554fb4cad37a/aries_cloudagent/revocation/routes.py#L1019):
```py
@response_schema(TxnOrRevRegResultSchema(), 200, description="")
async def send_rev_reg_def(request: web.BaseRequest):
    ...
    if not create_transaction_for_endorser:
        return web.json_response({"result": rev_reg.serialize()})

    else:
        ...
        return web.json_response({"txn": transaction.serialize()})
```

There are two return statements, providing either `rev_reg: IssuerRevRegRecord`, or `transaction: TransactionRecord`.

The problem seems to be the key "result" that's being used in the rev_reg response, which should presumably be "sent", in order to correctly map to the key in the `TxnOrRevRegResultSchema`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 10:58:24 +0000 UTC
    </div>
</div>

