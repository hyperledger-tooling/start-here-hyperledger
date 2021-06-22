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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Enhance blob upload support, to include metadata, and complete blob transfers (broadcast/private)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Build now takes releases of UI, rather than building during the docker build
  - See https://github.com/hyperledger-labs/firefly-ui/pull/37
- Blobs now can have both a `blob` attachment and `value` JSON
  - `data.blob.hash` - the sha256 of the blob - must be there
  - `data.blob.public` - the public payload ref to download the blob - only if it's been published at some point
- On upload user can add some extra form parameters - must be before the upload file itself:
  - `metadata` - can be a string or a JSON object
  - `autometa` - if `true` then the `filename`,`size` and `mimetype` are added to JSON metadata
     - Can be combined with `metadata` if the metadata is JSON
  - `datatype.name` - if the metadata needs to be validated per a datatype
  - `datatype.version` - if the metadata needs to be validated per a datatype
  - `validator` - to customize the validator (only `json` is supported today)
- The `hash` of the `data` object created, will be one of:
  - The `value` hash - if just a JSON value
  - The `blob` hash reference - if just a BLOB value
  - A hash of the two HEX hashes concatenated together (no spaces or separators)
- `GET` `/api/v1/namespaces/:ns/data/:dataid/blob` to download blob
   - Some refactoring on the apiserver to support non-JSON `ReadCloser` results
- Broadcast blob transfers worked through
  - When sent in a broadcast message, the `data` will become pinned
  - The `data` has a `blob.public` reference added to it before being included in the batch
  - If it's sent multiple times, to multiple parties, the upload to public only happens once
- Public payload references move to a `string` (rather than `*Bytes32`)
  - **This updates the contract Solidity** - so this has a migration impact for CLI created envs
  - We were previously using a Bytes32 reference, derived from the IPFS ID. This was problematic
    - It was really confusing on the plugin interface, and for users
    - It would have got more confusing with the public reference on data
    - It requires the public storage plugin to be able to translate IDs into 32byte strings
       - This happens to be true for the majority of IPFS configurations today, but is not universal or extensible
- Private blob transfers worked through
  - Sends are initiated prior to the batch payload itself
  - Happen asynchronously, and have their own `operation` entry
- E2E tests included
  - Private blob transfer
  - Broadcast blob transfer
     
Fixes #75
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 21:54:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    Get all config on admin, and support flat config records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - `/admin/api/v1/config` moved to `/admin/api/v1/config/records`
- `GET` `/admin/api/v1/config` added to download full merged config
- Fixed an error restarting when you set a non-object value in `/admin/api/v1/config/records`

In a PR chain with https://github.com/hyperledger-labs/firefly/pull/76
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 16:01:25 +0000 UTC
    </div>
</div>

