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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1838" class=".btn">#1838</a>
            </td>
            <td>
                <b>
                    0.7.4-rc5 changelog, version and ReadTheDocs updates
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
        Created At 2022-06-23 17:47:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1837" class=".btn">#1837</a>
            </td>
            <td>
                <b>
                    Allow setting a baseurl for the swagger urls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When deploying different agents on same gateway url in service mesh there occures some problem cause static swagger path und swagger.json has no unique uri. This PR enables a baseurl to be set for the swagger urls mentioned via the environment variable ACA_PY_BASE_URL:
Until now, the static swagger path and swagger.json path is always the default value set in setup_aiohttp_apispec (static/swagger for 'static_path' and /api/docs/swagger.json for 'url'). By setting the ACA_PY_BASE_URL, the path can now be adjusted so that the urls can be set to{ACA_PY_BASE_URL }/api/docs/swagger.json. The urls can then be easily resolved in the virtual service via unique urls.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 19:41:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1836" class=".btn">#1836</a>
            </td>
            <td>
                <b>
                    feat: make base wallet route access configurable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When adding admin routes through plugins, it makes sense for the plugin to be able to specify that those routes should be accessible to the base wallet when appropriate.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 19:14:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1834" class=".btn">#1834</a>
            </td>
            <td>
                <b>
                    Use local deps only
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 18:52:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1833" class=".btn">#1833</a>
            </td>
            <td>
                <b>
                    Improve typing of settings and add plugin settings object
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements some minor improvements on the type hints for the Settings classes and adds a class for `PluginSettings`. While working with plugins with configuration stored in ACA-Py's settings object, we often find ourselves needing to write lines like the following:

```python
value = cast(dict, context.settings.get(
    "plugin_config", {}
)).get(
    "my_plugin", {}
).get("value", DEFAULT_VALUE)
```

With this PR, we can now use:

```python
value = context.settings.for_plugin("my_plugin").get("value", DEFAULT_VALUE)
```
Or
```python
settings = context.settings.for_plugin("my_plugin")
value = settings.get("value", DEFAULT_VALUE)
```

The plugin settings object is immutable. This decision was made to encourage plugin authors to handle mutable values through either objects injected into the context on startup or by storing values in a record.

It's a minor quality of life tweak but this adds more structure to plugin configuration and value retrieval that I think was previously lacking while also improving readability.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 17:06:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1831" class=".btn">#1831</a>
            </td>
            <td>
                <b>
                    Enable pip-audit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 22:09:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1830" class=".btn">#1830</a>
            </td>
            <td>
                <b>
                    Update changelog and version for 0.7.4-rc4
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
        Created At 2022-06-21 22:02:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1829" class=".btn">#1829</a>
            </td>
            <td>
                <b>
                    Update pyjwt to 2.4
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
        Created At 2022-06-21 15:58:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1827" class=".btn">#1827</a>
            </td>
            <td>
                <b>
                    Fix IssuerCredRevRecord state update on revocation publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1823 broken in #1804

Ran against integration tests T002-TAA and T003-TAA which were previously failing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 22:16:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1824" class=".btn">#1824</a>
            </td>
            <td>
                <b>
                    Update POST /present-proof/send-request to POST /present-proof-2.0/send-request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

I got error messages when following the instructions and tried the updated version, which worked.

Signed-off-by: lineko <36633510+lineko@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 17:58:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1820" class=".btn">#1820</a>
            </td>
            <td>
                <b>
                    Fix: Present Proof v2 - check_proof_vs_proposal update to support proof request with restrictions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                - resolve #1755 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 14:10:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1818" class=".btn">#1818</a>
            </td>
            <td>
                <b>
                    Add troubleshooting document, include initial examples - ledger connection, out-of-sync RevReg
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
        Created At 2022-06-16 18:56:08 +0000 UTC
    </div>
</div>

