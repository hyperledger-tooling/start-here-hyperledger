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
                PR <a href="https://github.com/hyperledger/firefly/pull/1115" class=".btn">#1115</a>
            </td>
            <td>
                <b>
                    Fix typo in erc1155.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix typo in the erc155 tutorial init command. `ff init -t erc-1155` to `ff init -t erc1155`

Signed-off-by: Ander Dorado <71599694+ander-db@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-11 12:56:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1114" class=".btn">#1114</a>
            </td>
            <td>
                <b>
                    xdc + zksync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add xdc + zkSync tutorials
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 21:06:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1113" class=".btn">#1113</a>
            </td>
            <td>
                <b>
                    Dynamic configuration reload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Summary

This PR implements file-listener based dynamic configuration reload for FireFly Core.

- Allows listening for changes to a config file in a Kubernetes `configmap` or `secret`
- Performs analysis on the configuration to determine what `namespaces` and `plugins` have changed
  - Note: Does not currently support reloading API server configuration
- Does not affect any namespaces that are unaffected by changes
- Restarts all namespaces affected by plugin changes, or direct configuration changes
- Adds namespaces that did not previously exist
- Removes namespaces that have been removed

> Depends on https://github.com/hyperledger/firefly-common/pull/40 making it into a release before this can be merged

## Implementation detail

The `namespace.Manager` code has been refactored with the following significant changes:
- The initialization code has been decomposed into blocks that can be re-run during config reload
- A strong separation is created between configuration load+validation, and runtime initialization
- The individual maps of `namespaceManager.plugins` and `namespaceManager.pluginNames` has been replaced with a single map of `plugins` - which depending on the `category` will have a link to the specific plugin type
- A new dynamic configuration reload function is connected to a file listener, which tries to be self-explanatory as follows:
https://github.com/hyperledger/firefly/blob/1ffb555be43a788d40c624c29d421a6f0f931bc4/internal/namespace/configreload.go#L63-L124

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 06:19:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1112" class=".btn">#1112</a>
            </td>
            <td>
                <b>
                    Typo - change WebHooks to WebSockets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Spotted this reading the web hooks docs. Assume it should say "WebSockets"

Signed-off-by: Matthew Whitehead <matthew.whitehead@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 13:38:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1111" class=".btn">#1111</a>
            </td>
            <td>
                <b>
                    Add 'fetchstatus=true' query param to /operations/{opid}
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1108 

See related UI PR https://github.com/hyperledger/firefly-ui/pull/208 which uses this query parameter to populate a `Detail` section of the operation slide out.

Signed-off-by: Matthew Whitehead <matthew.whitehead@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 11:48:49 +0000 UTC
    </div>
</div>

