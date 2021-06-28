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
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    Sync/async bridge front-end
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes out the functional requirements in #81 

Core updates:
- New route: `POST` `/api/v1/namespaces/:ns/request/message`
   - Performs a request/reply exchange
   - Request is a `MessageInOut` in the body
     - Just like `.../send/message`
     - Data can be in-line or referenced
     - Requires `header.tag` to be set in message
   - Response is a `MessageInOut` in the body
      - Data is in-lined for you
- New event plugin called `system`
  - Simply delivers events to other components in the core
  - Cannot be disabled
  - Used with ephemeral events by the sync/async bridge
  - API prevents creation of durable subs externally on the transport
- Added `syncasync.Bridge` component
  - Included on periodic table as `[Sa]`
  - Only responsibility currently managing in-flight events
  - Could be extended to more gateway-like behavior in the future, taking arbitrary HTTP requests and encoding/propagating
- Added `filter.author` option on subscriptions
  - In pinned request scenarios, this allows the sender to exclude themselves from the list of responders
    - Without a filter on their subscription, they could attempt to respond to themselves
  - Currently only matters when the request is pinned
    - If a message is unpinned, there is no `message_confirmed` event on the sending party

Other enhancements:
- Fix to events where we could cross-emit on connections from the wrong transport
  - Resulted in `FF10190` `MsgMismatchedTransport` errors
  - Made significantly more likely by adding in the system events listener
- Adds `Request-Timeout` header to allow the client to customize the server-side timeout
  - No point the server waiting longer than the client is going to wait
  - Used header name from this old draft as basis: https://tools.ietf.org/id/draft-thomson-hybi-http-timeout-00.html
  - This is in addition to the config-based request timeout (default=2mins) we already have
- Removes requirement to include yourself in a group
  - If you omit yourself, the identity configured on the node will be added
  - You can still add a specific identity that's a child of that in multi-tenant scenarios
- Added more config on `webhooks` subscriptions, after from thinking through use cases
  - `input.replytx` - set the reply transaction type dynamically from the request
  - `input.path` - add a path suffix to the URL (performs safe escaping)
- Removes storing `group_hash` on events
  - Was unnecessary as we already have filters on message specific items, and bloats events table
  - No need for a migration to remove it on existing envs
- Renames `MessageInput` to `MessageInOut` as it was confusing using it on output before
  - Also moved the helper to add data to a response to `fftypes` so it's in one place
- Fixed the Schema generation for the OpenAPI on create subscriptions
  - Previously it had all the dynamic options at top level, whereas they should be under `options`
- Change e2e test to teardown before building the docker image
  - Seemed to be necessary after recent CLI changes, which meant `ff remove` was deleting images
- Updated e2e test to include request/reply example
  - Replaced the old NoTx exchange test
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 02:02:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/98" class=".btn">#98</a>
            </td>
            <td>
                <b>
                    Add publicURL config to admin and http config, and file based logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Public URL
    - Adds config option for cases where the listener address (such as `0.0.0.0`) is not the same as the URL that should be used externally for FireFly.
    - This affects the Swagger UI, which needs to perform an call from the browser to download the Swagger YAML.
- File logging
    - Uses lumberjack writer
    - Adds following config options:
    - `log.filename` - filename to log to
    - `log.maxAge` - maximum age before rotating
    - `log.maxSize` - maximum size
    - `log.maxBackups` - maximum number of files to keep
    - `log.compress` - whether to compress the backups
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 01:55:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/97" class=".btn">#97</a>
            </td>
            <td>
                <b>
                    Add workflow for E2E test
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
        Created At 2021-06-24 00:50:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Fix ordering of message checks in TestE2EWebhookExchangeNoTx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #94 fixed the order of the request and reply, but the e2e test was depending on the incorrect order (noting natural sort order is newest first)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 21:42:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    Fix pending unpinned sends
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently if you send an unpinned message, it is correctly marked `pending: false` (with a confirmed timestamp) on the receiving node(s), but the sending node leaves it forever in a `pending` state on the sender.
This means in the UI, all the requests are shown _before_ the replies 🙃 

The problem was the unpinned send code was setting `pending` and `confirmed` _before_ sealing the message, which then reset those back to default.

![image](https://user-images.githubusercontent.com/6660217/122996051-6345ff00-d378-11eb-91b2-19bd3d7c2e37.png)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 20:41:22 +0000 UTC
    </div>
</div>

