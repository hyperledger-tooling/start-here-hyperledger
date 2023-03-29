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
                PR <a href="https://github.com/hyperledger/firefly/pull/1242" class=".btn">#1242</a>
            </td>
            <td>
                <b>
                    Re-establish active subscriptions after dynamic Namespace reload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                On a dynamic reload of an _existing_ namespace (for example if there's a tweak to the config) the old namespace is stopped, and all subscription event polling associated with that namespace is stopped,

However, for WebSockets events there is currently no trigger to restart the listeners.

In this `connect-in` case of Events, the Orchestrator relies upon a `RegisterConnection` function call from the Events plugin, when the `start` command comes over the WebSocket to from the application.

In this case the application never disconnects/reconnects... so there's no new `start` payload.

So this PR proposes a new `NamespaceRestarted` function call from Orchestrator _to_ the Events plugin, which then becomes responsible for making new `RegisterConnection` calls for all active subscriptions.

To make this safe to happen on every startup, asynchronously to connections coming in, a timestamp is passed to the `NamespaceRestarted` so it can only re-register connections that came in before the restart time.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 11:47:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1240" class=".btn">#1240</a>
            </td>
            <td>
                <b>
                    Add GitHub issue templates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding some issue templates to guide people to Discord for questions and support.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-27 17:40:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1236" class=".btn">#1236</a>
            </td>
            <td>
                <b>
                    Add an indxed column and simple query API for distinct sub-paths
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1227 

- Adds a `blob_path` column / `blob.path` JSON field for the path
- Standardizes on `/` prefixing on these paths, without requiring the name to include a `/` prefix
- Provides a simple API for querying the direct decendents of a path (no pagination or filtering, simple string return)

> This **only** adds the column for newly created data objects, and it will be empty for all existing data

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-26 21:03:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1235" class=".btn">#1235</a>
            </td>
            <td>
                <b>
                    Fix archive name for integration test logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes the name of the uploaded log archives from each E2E run. The `blockchain-node` variable was not set, so it was an empty string, causing name collisions. This means that we are missing detailed logs from certain runs, making it hard to debug integration failures.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 15:41:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1234" class=".btn">#1234</a>
            </td>
            <td>
                <b>
                    Validate and restore listeners on startup, and allow deletion if not found in connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Had a situation where we wanted to restore fresh listeners for custom contracts on a FireFly core service, and had assumed FireFly core would re-create the listeners. So deleted them on the EVMConnect runtime directly and restarted FF.

Found related issues, that meant we had to go into the FF DB and remove the contract listeners directly (and have the app recreate them):
1. FireFly did not recreate the listener. This seems a little inconsistent with both the `BatchPin` listener, and the listeners of the token connectors...
   - Proposing in this PR that we automatically recreate the listeners where possible (only Ethereum in this PR, due to existing limitations around the Fabric connector integration where it does not have existing query support to check existence)
2. The API could not be used to delete the listener, because when EVMConnect returned a `404` FireFly failed the `DELETE` API.
    - This seemed like a straight bug to me. Due to the return of status being `interface{}` and the complexity of a `nil` check there, we're adding an extra `bool` to whether it's found or not (Fabric always returns true)
3. Found in testing this change, that the check on existence of a contract listener with the same parameters was not working, passing in a `[]byte` for the `location` rather than `string`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 22:44:02 +0000 UTC
    </div>
</div>

