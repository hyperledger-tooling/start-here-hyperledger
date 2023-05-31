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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2247" class=".btn">#2247</a>
            </td>
            <td>
                <b>
                    chore!: drop python 3.6 support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update setup.py minimum python version requirement.
Update workflows to use Python 3.9 by default.
Update container image docs.

@swcurran @WadeBarnes I believe these are the relevant changes in workflows and setup files in order to officially drop Python 3.6. I think once we've made the transition, there are a number of dependencies that ought to be updated. I think those updates are best suited to a follow up PR.

closes: #2244 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-27 20:01:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2246" class=".btn">#2246</a>
            </td>
            <td>
                <b>
                    Upgrade codegen tools in `scripts/generate-open-api-spec` and publish Swagger 2.0 and OpenAPI 3.0 specs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now is as good a time as any to upgrade the codegen tools in `scripts/generate-open-api-spec` to use the latest `swaggerapi/swagger-codegen-cli` release (it was ~3 years out of date). 

Additionally, I added the latest `openapitools/openapi-generator-cli`, so that the spec generation now provides both a Swagger 2.0 spec, and an OpenApi 3.0 spec. This way users don't need to manually upgrade the spec themselves.

Previously the Swagger 2.0 spec was simply called `openapi.json`. This is now renamed `swagger.json`, with the 3.0 compatible spec in its place. 

Worth noting that the spec validation still only throws warnings that can be ignored:
- the `swagger` spec validation only complains about some missing operationId's (and 'host' not defined);
- and the `open-api` spec validation only complains about `example` fields being unexpected, and a single case of `attribute tags.tagsexternalDocs.url is missing`.

Also, I updated the `UsingOpenAPI.md` file to reflect these changes, with some minor neatening up included.

Review can be validated by running `scripts/generate-open-api-spec`.

Discussion re further edits is welcome.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-27 12:01:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2245" class=".btn">#2245</a>
            </td>
            <td>
                <b>
                    ./run_demo performance -c 1 --mediation --timing --trace-log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bug with prompt_toolkit and trace logging. Could only bump up the prompt_toolkit library so much since demos run on Python 3.6. However, I did attempt on 3.9 with the latest version of prompt_toolkit and setting an env var (see https://github.com/prompt-toolkit/python-prompt-toolkit/pull/898). This still did not correct the issue, so reverted to existing code and just handled the exception(s). The output of the trace log is being written to the console, my limited understanding of this would be that the trace log works, but also triggers the prompt_toolkit to do the same work and gets into conflict.

Fixes #2205 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 17:21:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2243" class=".btn">#2243</a>
            </td>
            <td>
                <b>
                    fix: route multitenant connectionless oob invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This addresses an issue where the keys used in connectionless oob invitations were not correctly set-up for routing through the base wallet when multi-tenancy is enabled, which resulted in those invitation not being usable.

cc @lohanspies @ff137


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 12:49:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2241" class=".btn">#2241</a>
            </td>
            <td>
                <b>
                    Feat: Added support for Ed25519Signature2020 signature type
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
        Created At 2023-05-25 15:37:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2240" class=".btn">#2240</a>
            </td>
            <td>
                <b>
                    fix: only cache completed connection targets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adjusts the caching behavior for connection targets to solve some issues seen in multi-replica setups under certain circumstances.

### The Problem

Given the following conditions,
- ACA-Py is connecting to a remote agent through the remote agent's Public DID
- ACA-Py is using more than one replica with loadbalancing such that one replica may start a DID Exchange/Connection and another may finish the exchange.
- Following connection, ACA-Py attempts to issue a credential to the remote agent (or theoretically any other message where the protocol requires a connection)

If the agent that initiates the credential issuance is not the same agent that completed the DID exchange, the agent will have a connection target cached that still contains the public DID and public routing info of the remote agent, causing the remote agent (if it's also running ACA-Py) to get errors like the following:

```
2023-05-23 18:18:55,358 aries_cloudagent.core.conductor ERROR Exception in message handler:
Traceback (most recent call last):
  File "/usr/lib/python3.9/asyncio/tasks.py", line 256, in __step
    result = coro.send(None)
  File "/usr/lib/python3.9/site-packages/aries_cloudagent/core/dispatcher.py", line 264, in handle_message
    await handler(context, responder)
  File "/usr/lib/python3.9/site-packages/aries_cloudagent/protocols/issue_credential/v2_0/handlers/cred_offer_handler.py", line 51, in handle
    raise HandlerException(
aries_cloudagent.messaging.base_handler.HandlerException: No connection or associated connectionless exchange found for credential offer
```

This is because it received a message encrypted for it's public DID and key, which does not have a connection associated with it.

Consider the following diagram. In this diagram, `alice0` and `alice1` represent two replicas of ACA-Py working collectively to represent an Alice agent. `bob` represents the remote agent.

![offer-cred-cache-conn-failure](https://github.com/hyperledger/aries-cloudagent-python/assets/22032832/a9c36980-04ed-4704-9b35-2c49cd20b15c)

If the loadbalancing of the replicas happens to cause the above handling of messages by the different replicas, we see the error pasted above on `bob`.

This can also happen with a slightly different sequence of messages, as shown in this diagram:

![issue-cred-cache-conn-failure](https://github.com/hyperledger/aries-cloudagent-python/assets/22032832/5ed1b63e-2273-4484-b706-2da01954e9ea)

In this case, this results in the following error on `bob`:

```
Traceback (most recent call last):
  File "/usr/lib/python3.9/asyncio/tasks.py", line 256, in __step
    result = coro.send(None)
  File "/usr/lib/python3.9/site-packages/aries_cloudagent/core/dispatcher.py", line 264, in handle_message
    await handler(context, responder)
  File "/usr/lib/python3.9/site-packages/aries_cloudagent/protocols/issue_credential/v2_0/handlers/cred_issue_handler.py", line 49, in handle
    raise HandlerException(
aries_cloudagent.messaging.base_handler.HandlerException: No connection or associated connectionless exchange found for credential
```

### The Solution

The solution implemented by this PR is to only cache connection targets on completion of a DID Exchange or connection; or, in other words, only cache connection targets for connections that have reached a `completed` state. Given that the connection target is intentionally changed in the process of these protocols (you could even say that's kind of the whole point of the protocol), I believe there is little benefit to caching the initial connection target anyways. This notion is supported by these lines:

https://github.com/hyperledger/aries-cloudagent-python/blob/main/aries_cloudagent/connections/models/conn_record.py#L503-L513

```
    async def post_save(self, session: ProfileSession, *args, **kwargs):
        """Perform post-save actions.

        Args:
            session: The active profile session
        """
        await super().post_save(session, *args, **kwargs)

        # clear cache key set by connection manager
        cache_key = f"connection_target::{self.connection_id}"
        await self.clear_cached_key(session, cache_key)
```

After every save on the connection record (which will occur at basically every step of the did exchange or connection protocols), we're clearing the cache of the target.

Given that the cache is being cleared, causing the connection target info to be recalled from the wallet record, I believe the changes made in this PR should not impact performance, though I have not tested this.

I get the feeling this change could improve other scenarios we've seen previously that motivated the creation of the redis cache plugin but I have not tested these other scenarios.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-24 16:29:47 +0000 UTC
    </div>
</div>

