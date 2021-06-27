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

