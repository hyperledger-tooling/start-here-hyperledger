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
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    Add README link for firefly-samples
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
        Created At 2021-06-29 22:00:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/103" class=".btn">#103</a>
            </td>
            <td>
                <b>
                    update ui to release v0.1.2
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
        Created At 2021-06-29 15:33:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/102" class=".btn">#102</a>
            </td>
            <td>
                <b>
                    Local docs build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add a build that you can run on your laptop with: `bundle exec jekyll serve`
- Add a link to the docs from the readme
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 21:20:32 +0000 UTC
    </div>
</div>

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

