---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/896" class=".btn">#896</a>
            </td>
            <td>
                <b>
                    Support tokens only namespaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now, multiparty-disabled namespaces can run without a blockchain plugin:
 * All contract routes will be disabled
 * Identity normalizations that rely on a blockchain plugin will either default to the specified input/default key or fail
 * `aggregator` is not started within `EventManager`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 14:40:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/895" class=".btn">#895</a>
            </td>
            <td>
                <b>
                    Map namespace between local name and remote name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)

Orchestrator is now aware of the namespace local name _and_ remote name, as are some of the managers. Plugins are intentionally not aware of the mapping, but are passed the local or remote namespace names as appropriate.

The only two items which _record_ a remote namespace name are `Message` and `Group`. These now have an additional `localNamespace` field, which will be populated with the local namespace, while the existing `namespace` field will be populated with the remote namespace (because it is part of the hash in both of these cases, it must remain the same for all members). In addition, `Batch` and `Data` items will be populated with the remote namespace name for network transit (but will be stored with the local namespace name only). Beyond these, every other existing object simply continues to populate its `namespace` with a local namespace name.

Some more notes on how the local namespace is filled for other items:
* All definition types (datatypes, contract FFIs/APIs, identities, and token pools) are transmitted _without_ a namespace filled. Each receiving node will map the definition based on the enclosing message's namespace, and then will fill in the local namespace name before storing the item.
* Token transfers and approvals continue to inherit their namespace from the associated token pool.
* Contract listeners are still local-only, and blockchain events tied to them will inherit their namespace.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 20:39:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/894" class=".btn">#894</a>
            </td>
            <td>
                <b>
                    Add basic auth support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds basic auth support for:

- HTTP listeners
- All HTTP requests within a namespace (including WebSocket upgrades)
- `start` requests over an open WebSocket connection

Example config:

```
plugins:
  auth:
  - name: basicauth
    type: basic
      basic:
        passwordfile: /etc/firefly/allowed_users
```
Where `passwordfile: /etc/firefly/allowed_users` is a file created with `htpasswd` using bcrypt hashed passwords. For example, you can create such a file by running: 
```
htpasswd -cB allowed_users firefly
```

Prerequisites for merge:
- [ ] https://github.com/hyperledger/firefly-common/pull/24
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 19:19:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/893" class=".btn">#893</a>
            </td>
            <td>
                <b>
                    Add sqlite to Docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's helpful to have this handy when debugging database contents.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 16:19:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/892" class=".btn">#892</a>
            </td>
            <td>
                <b>
                    Fix logs from E2E test invocation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Disable parallelization and reduce test timeout to 1m.

This re-enables streaming logs during E2E runs (which is disabled by default when running suites in parallel). No real impact since our test jobs are already divided such that they run 1 suite per job.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 16:18:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/891" class=".btn">#891</a>
            </td>
            <td>
                <b>
                    Custom contract subscriptions now utilize namespaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">migration_consideration</span>
            </td>
            <td>
                Now, both ethconnect and fabconnect subscription names contain the namespace name. This means that events will now be delivered only to the callback handler for that namespace, instead of every single callback handler. Older subscriptions will still be delivered to all handlers. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 22:45:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/890" class=".btn">#890</a>
            </td>
            <td>
                <b>
                    Change default contracts to network version 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)

Split out separate "pinBatch" and "networkAction" methods in the V2 contract, and make it the default. Adjust the blockchain plugins to handle both versions of the contract cleanly.

Also fix some bugs found along the way with network actions being broken.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 18:32:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/889" class=".btn">#889</a>
            </td>
            <td>
                <b>
                    back port of "FAQ and FireFly Tutorial Updates"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                back port of #857 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 01:18:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/887" class=".btn">#887</a>
            </td>
            <td>
                <b>
                    Add E2E tests for gateway mode
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
        Created At 2022-07-06 19:46:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/886" class=".btn">#886</a>
            </td>
            <td>
                <b>
                    update token connector versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alex Shorsher <alex.shorsher@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 19:42:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/885" class=".btn">#885</a>
            </td>
            <td>
                <b>
                    back port of custom URI support for non-fungible tokens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                back port of https://github.com/hyperledger/firefly/pull/879 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 16:26:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/884" class=".btn">#884</a>
            </td>
            <td>
                <b>
                    Stop orchestrator for ff_system when moving to network V2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)
~~In a chain with #883~~
In a chain with #890

Background: The legacy `ff_system` namespace is created (ie an orchestrator and managers are initialized) whenever the default namespace is a V1 multiparty network. The `ff_system` namespace is initialized with an exact duplicate of the default namespace config (same plugins, same contract addresses, etc).

With this PR, if the default namespace (and therefore `ff_system`) migrates to V2 rules, the `ff_system` orchestrator will be stopped and removed, along with all its children.

This should allow legacy networks to cleanly migrate to V2 rules and retire `ff_system`. Notable caveat: once the default namespace is on V2, no other V1 namespaces will be supported.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 01:13:35 +0000 UTC
    </div>
</div>

