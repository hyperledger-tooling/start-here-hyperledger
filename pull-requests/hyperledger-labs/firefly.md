---
layout: default
title: firefly
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/65" class=".btn">#65</a>
            </td>
            <td>
                <b>
                    Updates to private messaging from e2e testing with CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves a few nits in the end-to-end flow:
- Ensuring the group creation event is created, and included in the same namespace as the first message on that group
- Making a batch rewind wake up the event poller immediately, to assemble the message
- Generate a `group_confirmed` event only (no separate `message_confirmed`) when a group arrives
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 22:55:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/64" class=".btn">#64</a>
            </td>
            <td>
                <b>
                    fix proposal link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nick Gaski <nick.gaski@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 21:24:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/63" class=".btn">#63</a>
            </td>
            <td>
                <b>
                    Fix E2E test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This gets the E2E test running again with the latest API. Can (should) be run manually before commits with `./test/e2e/run.sh`. Eventually will get it added to a GitHub action as well.

It's not as clean or as thorough as it could be, but it's a start. Feedback/future suggestions welcome.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 21:02:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/62" class=".btn">#62</a>
            </td>
            <td>
                <b>
                    Add status API endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `GET` `/api/v1/status` returns a structure containing:

- Org information - name, identity, whether it's registered, and if so what the ID is
- Node information - name, whether it's registered, and if so what the ID is
- Defaults - just the default namespace for now
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 15:42:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/61" class=".btn">#61</a>
            </td>
            <td>
                <b>
                    Rename the go package name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 13:54:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    Config API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a new `/config` endpoint which can be used for dynamically adding or modifying config at runtime via a REST API. Any change in configuration will result in a restart of all services and plugins (not the process itself though).

Due to how powerful (dangerous) the new configuration endpoints are, they have been moved to a separate “admin” HTTP listener which will listen on a separate port, if enabled at all. By default, it is disabled. To enable the admin endpoints, add the following lines to your firefly.core config:

```yaml
admin:
  enabled: true
  address: 0.0.0.0
  port: 5001
```

To set a configuration key make a `PUT` request to `/admin/api/v1/config/{key}` with a JSON request body.


For example, if you want to set the HTTP URL for ethconnct, you would make a `PUT` request to `/admin/api/v1/config/blockchain.ethereum.ethconnect` with a request body of:

```json
{
  "url": "http://some_url"
}
```

The payload will be merged with any existing config. This means that it is not possible to _remove_ configuration keys that are present in the config file, via the REST API.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 01:08:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    Add Docker Build GitHub Action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a new GitHub Action that builds and pushes Docker images to GitHub Container Repository.

It also re-enables our normal PR checks after the repo was transferred.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 22:55:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/58" class=".btn">#58</a>
            </td>
            <td>
                <b>
                    Update links in README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated links to match new repo URLs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 22:19:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    Update GitHub URL for firefly-ui
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 20:36:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    Firefly -> FireFly in docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 20:19:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    Rename kld query strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 19:41:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/53" class=".btn">#53</a>
            </td>
            <td>
                <b>
                    initial docs library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nick Gaski <nick.gaski@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 19:10:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Add private send API route
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Example `POST` to `/api/v1/namespaces/{ns}/send/message`

```json
{
  "data": [{
      "value": "hello world"
  }],
  "group": {
    "members": [
      {"identity": "org_0"},
      {"identity": "org_1"}
    ],
    "name": "mygroup1"
  }
}
```

There are a few bug fixes in the PR from testing end to end, particularly around ensuring the groupid propagates through the layers where it needs to.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 21:37:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/48" class=".btn">#48</a>
            </td>
            <td>
                <b>
                    Fix logic for querying "local" flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 15:23:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    HTTP Data Exchange plugin connections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fills out the Data Exchange interfaces
  - Get endpoint info (to broadcast)
  - Add peer (from broadcast)
  - Upload blob (streaming interface - ns+UUID)
  - Download blob (streaming interface - ns+UUID)
  - Send message (in-line bytes)
  - Send blob (must already be uploaded - not yet fully integrated with core in this PR)

- Implements the integration with https://github.com/kaleido-io/firefly-dataexchange-https
  - HTTPS + WebSockets using the standard clients already built into core

- Implements batch off-chain message transfer
  - Messages are used for the transfer of the `batch` data
  - The heavy lifting was already complete in #42, so this just joins the dots of sending data and processing events

- Nodes now have `name` and `owner` (not an identity)
  - This is because for Data Exchange, there is a `peerID` as well. So it's not possible to reconcile a single identity with a node
  - So now instead when a message arrives over the private data exchange, we can use the `peerID` to lookup the node, and then resolve the identity matching that
  - We traverse up the tree, so if a batch arrives signed by an org, and that org has a parent, we are will to accept that message from any node that is owned by any org as you move up the hierarchy.

- Groups no longer have a UUID (or a description)
  - Instead are identified via a `hash` combining:
    - The list of members
    - The ledger (Fabric channel etc.)
    - An application specified `name`
  - This means all referring objects, like `Message` etc. now use a Bytes32 rather than UUID to refer across
  - This was important, to allow applications to simply define+use groups without waiting for propagation and agreement on which ID wins. Now it doesn't matter which group initiation message is sent first, as all the definitions are the same, and the later ones will be ignored. It just matters that the same member list is used in each. The name is optional.

- Rewind support for the event aggregator in the case of off-chain data arriving after a batch pin on-chain TX
  - Simply rewinds the `offset` back to the earliest offset in the batch that arrived
  - We re-process any `pin` entries since then, that aren't already marked `dispatched`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 14:51:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    add namespace filter to TransactionFactory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - allows transaction queries to be filtered by namespace
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 14:27:32 +0000 UTC
    </div>
</div>

