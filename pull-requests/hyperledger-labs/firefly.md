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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    Wait to reset parent context after HTTP request context finishes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes HTTP requests sometimes failing when resetting FireFly after a config change.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 13:56:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    Unpinned message transfer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Adds a transport wrapper to DX messages, to allow different payloads with efficient deserialization
- Allows an individual unpinned message and data array to be sent, as well as pinned batches
- Adds the group to the private send, so it can be created on the far side
  - The sending side (only) still does a groupinit pinned to the chain, but it's completely async to the private exchanges
- Requires the transaction type of that message to be `none` and the sender to be valid
- Immediately confirms the message and triggers the event
- E2E test included
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 13:05:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/89" class=".btn">#89</a>
            </td>
            <td>
                <b>
                    Webhooks event interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ticks off key half of #81 
- Adds a new `webhooks` event transport
- Add plugin option to add custom documented options to subscriptions
- Add plugin interface to send replies
- Additional base option added as follows for subscription:
  - `withData` (boolean) - resolve the data of the message to pass to the event
- The new transport has the following custom options:
  - `reply` (boolean) - whether to reply
  - `replytag` (string) - the `tag` to use in the reply message
  - `fastack` (boolean) - when true does not wait for HTTP call to complete to ack (meaning parallelism)
  - `url` (string) - the URL to call
  - `method` (string) - the HTTP method to invoke
  - `json` (boolean) - whether to assume the response is JSON, even if the content-type is not set
    - Non-JSON payloads are returned as base64, as per the e2e test
  - `headers` (map string->string) - static headers to set on the request
  - `query` (map string->string) - static query params to set on the request
  - `input.query` (string) - field to reference on the first JSON data in the input message event, to add query params
  - `input.headers` (string) - field to reference on the first JSON data in the input message event, to add headers
  -  `input.body` (string) - field to reference on the first JSON data to be the data
- Includes diagnosis/fix for PSQL constraint issue in #90

In PR chain with #80 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-20 16:57:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    Add config options for ethconnect prefix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds configuration options for the `ethconnect` plugin:

- `shortPrefix`: used in query parameters in requests to `ethconnect`
- `longPrefix`: used in x-headers in requests to `ethconnect` if headers are used in the future
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 21:16:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/87" class=".btn">#87</a>
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
                Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 18:56:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/86" class=".btn">#86</a>
            </td>
            <td>
                <b>
                    Fix QL migration for batches
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes an inconsistent DB constraint between the QL schema and the PostgreSQL schema, which is causing errors when using QL.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 16:46:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/85" class=".btn">#85</a>
            </td>
            <td>
                <b>
                    Call Reset() before reading config on startup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should fix default values not getting applied at startup.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 18:23:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/82" class=".btn">#82</a>
            </td>
            <td>
                <b>
                    Do not auto-reset, and add preinit mode requiring at least one config record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add a `POST` `/admin/config/reset` to initiate the reset separately from adding config records
- Add an `admin.preinit` option such that if there are no config records, a server will only start the admin server and not attempt to initialize. This means it will wait for the first config+reset to be `PUT` to it before attempting to start
- Added fix to https://github.com/hyperledger-labs/firefly/issues/79
  - In addressing this, I made some progress on the refactor discussed in https://github.com/hyperledger-labs/firefly/pull/51#issuecomment-857957200

Fixes #79
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 21:34:55 +0000 UTC
    </div>
</div>

