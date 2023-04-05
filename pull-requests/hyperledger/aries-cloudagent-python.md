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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2204" class=".btn">#2204</a>
            </td>
            <td>
                <b>
                    Add Explicit/Offline marking mechanism for Upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2201 
- Pending extensive testing with docker-test scripts

In the config, `explicit_upgrade` is the flag or key and it's value can be `critical` [meaning error and stop] or `warning` [log and proceed]. ~~With `warning`, if there are versions which are not marked as explicit and are in scope for applying the upgrade then upgrade for these versions will proceed [after that it will continue the ACA-Py start up process].~~ With warning, if there are version which are not marked as explicit and are in scope for applying the upgrade then no upgrade will be performed and version in storage not updated.

```
"v0.7.2": {
    ...,
    "explicit_upgrade": "warning",
},
"v0.7.3": {
    ...,
    "explicit_upgrade": "critical",
},
"v0.7.1": {
    ...,
},
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 02:52:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2203" class=".btn">#2203</a>
            </td>
            <td>
                <b>
                    Change upgrade definition file entry from 0.8.0 to 0.8.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

Fixes #2202 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 19:55:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2200" class=".btn">#2200</a>
            </td>
            <td>
                <b>
                    Add Upgrading ACA-Py document
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
        Created At 2023-04-04 19:08:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2198" class=".btn">#2198</a>
            </td>
            <td>
                <b>
                    0.8.1-rc2
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
        Created At 2023-04-03 21:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2196" class=".btn">#2196</a>
            </td>
            <td>
                <b>
                    Fix: Indy WalletAlreadyOpenedError during upgrade process
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2195 
- resolve #2197 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 15:16:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2194" class=".btn">#2194</a>
            </td>
            <td>
                <b>
                    0.8.1-rc1
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
        Created At 2023-03-31 20:41:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2193" class=".btn">#2193</a>
            </td>
            <td>
                <b>
                    Fix: Resolve Upgrade Config file in Container
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2192 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 19:54:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2191" class=".btn">#2191</a>
            </td>
            <td>
                <b>
                    feat(WIP): anoncreds updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a significant refactor of ACA-Py's handling of Anonymous Credentials, switching to the ledger-agnostic anoncreds-rs library instead of Indy specific libraries we've been using up until this point.

This PR is a work in progress. Given that ACA-Py has been built with Indy-isms and Indy specific libraries since the beginning, there's a lot that needed to be touched in order to move towards a more ledger-agnostic mentality. As of the time of opening this PR, it includes:

- A pluggable interface for defining AnonCreds Method Plugins, enabling resolution or registration of AnonCreds objects on any ledger/network/resolvable location as long as there is a plugin that implements it.
- A new set of Admin API endpoints for creating AnonCreds objects in a ledger-agnostic, plugin-friendly way
- Replaced indy-shared-rs with anoncreds-rs (indy-shared-rs still getting installed but not used)
- Added builtin plugins for:
  - Legacy Indy (Identifiers not using did:indy urls)
    - Supports registering and resolving Schemas and Credential Definitions; revocation objects are WIP
  - did:indy - Currently just stubbed out
  - did:web - Currently just stubbed out
- A simple demo script (to be removed and replaced with proper Integration tests) demoing issuance and verification (without revocation currently) on Legacy Indy.
  - This can be run with `docker-compose run tests && docker-compose down -v`

We are actively working on:
- Implementing revocation support through the new AnonCreds interface

Things that are very broken right now:
- The old `/schemas` and `/credential-definitions` endpoints
- Revocation
- Endorsement
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 17:46:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2190" class=".btn">#2190</a>
            </td>
            <td>
                <b>
                    0.8.1-rc0
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
        Created At 2023-03-31 02:07:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2189" class=".btn">#2189</a>
            </td>
            <td>
                <b>
                    Doc update and some test scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update to the plug-in docs

A couple of docker scripts for running aca-py and a postgres database

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 21:30:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2187" class=".btn">#2187</a>
            </td>
            <td>
                <b>
                    3.7 and 3.10 unittests fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Disabled two tests related to this issue. Not sure on the resolution in the future. 
https://github.com/hyperledger/aries-cloudagent-python/issues/2072#issuecomment-1489279654

Updating two other dependencies resolved the other issues. See successful test run in my fork.
https://github.com/Jsyro/aries-cloudagent-python/actions/runs/4568725894/jobs/8064139393
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 21:10:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2185" class=".btn">#2185</a>
            </td>
            <td>
                <b>
                    Update and automate ACA-Py upgrade process
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2181 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 17:53:55 +0000 UTC
    </div>
</div>

