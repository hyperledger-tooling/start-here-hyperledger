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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1352" class=".btn">#1352</a>
            </td>
            <td>
                <b>
                    fix: deepcopy attach decorator data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @Moopli had an interop issue between AFGO and ACA-Py. It came down to ACA-Py modifying the json returned from an attachment decorator which would cause issues later on because the object was missing some expected properties. (see more info below)

To prevent such mistakes in the future it is now fixed by making a deep copy both when setting and retrieving json from an attachment decorator. I'm not 100% what the impact of this is on performance, and whether json.dumps and json.loads may be faster.

We could also fix it by making a copy in the json ld handler, but this won't fix the issue all together. @andrewwhitehead I'm interested to hear which approach you'd take.

> TimoGlastra I found the bug
from here:
https://github.com/hyperledger/aries-cloudagent-python/blob/main/aries_cloudagent/protocols/issue_credential/v2_0/manager.py#L571
we end up calling ld_proof/handler LDProofCredFormatHandler.receive_credential, and when it gets here:
https://github.com/hyperledger/aries-cloudagent-python/blob/main/aries_cloudagent/protocols/issue_credential/v2_0/formats/ld_proof/handler.py#L493
it modifies the original attachment in the message, removing the proof member from the credential. So when the ld proof handler returns, V20CredManager stores the damaged message, causing the later error on deserialization.
The issue is, AttachDecorator returns json attachments by reference: https://github.com/hyperledger/aries-cloudagent-python/blob/main/aries_cloudagent/messaging/decorators/attach_decorator.py#L560
To fix this issue alone, LDProofCredFormatHandler.receive_credential could simply build a shallow copy of cred_dict
but I imagine that where one bug appears, others lurk in silence - is AttachDecorator` supposed to provide a mutable reference? Or should it return a deep copy of the dict?
the workaround I'm doing right now is to make the issued credential a b64 attachment instead
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 20:33:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1350" class=".btn">#1350</a>
            </td>
            <td>
                <b>
                    Poc multitenant profiles
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
        Created At 2021-08-11 13:56:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1348" class=".btn">#1348</a>
            </td>
            <td>
                <b>
                    Refactor outbound queue interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adjusts the outbound queue interface to be more easily generalized. As we've worked to implement outbound queuing via Kafka, we've found that the configuration just did not map onto what was needed in Kafka. Rather than expecting a connection string and parsing protocol etc. etc., this PR just passes all settings to the outbound queue implementation and allows it to read plugin configuration from the settings. This affords much greater flexibility in the structure of the outbound queue implementation. As a result, I removed some outbound queue command line arguments that were no longer used.

Additionally, I updated aioredis to 2.0.0. From the aioredis maintainers speaking on version 1.3.1 of the library:

> As of December, 2019, this library had been abandoned. The code had grown stale, issues were piling up, and we were rapidly becoming out-of-date with Redis’s own feature-set. In light of this, the decision was made to ensure that the barrier to support for potential maintainers or contributors would be minimized.

I found that using aioredis 2.0.0 significantly simplified the code as it stood.

Some other minor consistency fixes were made to bring the outbound queue package in line with the rest of the code base.

I haven't had an opportunity to integration test the redis changes just yet. I noticed there were some tests for this but they did not appear to be run anywhere in the tests run by the github actions. Is this something we would want run as part of PR checks or is the occasional one-off sufficient?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 02:55:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1347" class=".btn">#1347</a>
            </td>
            <td>
                <b>
                    feat: set arbitrary plugin config value at cli
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Doing a bit of spit balling.

We previously addressed the need for supplying configuration to plugins with the `--plugin-config` flag to load a yaml file into `settings` for use by plugins. We've found this feature to be quite helpful, especially in the case of loading multiple plugins (i.e. resolvers) that each require their own configuration. However, we have also found that it would be handy to be able to set or modify these values from the command line. So instead of having to modify the `plugin_config.yml` you're using to load the universal resolver plugin to point it to a different resolver instance, we could have a command line argument like the following:
```
--plugin-config-value http_uniresolver.endpoint=http://localhost:3000
```

Or perhaps a short form of:
```
-o http_uniresolver.endpoint=http://localhost:3000
```

With such a command line argument, we propose that dotted key values act as a shorthand for nesting values. For example, `a.b.c.d=value` becomes `{"a": {"b": {"c": {"d": "value"}}}}`. We also propose that the value be loaded as yaml to avoid parsing ourselves while still allowing us to express values more complicated than just strings and numbers.

Open to thoughts :slightly_smiling_face: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 00:35:28 +0000 UTC
    </div>
</div>

