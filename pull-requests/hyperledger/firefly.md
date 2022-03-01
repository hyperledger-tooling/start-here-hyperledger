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
                PR <a href="https://github.com/hyperledger/firefly/pull/555" class=".btn">#555</a>
            </td>
            <td>
                <b>
                    Explicitly name all subscriptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #554 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 23:33:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/553" class=".btn">#553</a>
            </td>
            <td>
                <b>
                    Documentation updates from @TheSwarnim
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a build fix to https://github.com/hyperledger/firefly/pull/451
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 18:14:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/552" class=".btn">#552</a>
            </td>
            <td>
                <b>
                    Docs "bundle update" to pick up new nokogiri build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves a dependabot notification: https://github.com/hyperledger/firefly/security/dependabot/7
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 18:11:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/551" class=".btn">#551</a>
            </td>
            <td>
                <b>
                    Roll requestConflictEmptyResult from Group to Data and Message too
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #550

The comment in https://github.com/hyperledger/firefly/pull/513#issuecomment-1036844541 held true - we need to roll the `requestConflictEmptyResult` tweak out to the other optimization cases.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 17:58:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/549" class=".btn">#549</a>
            </td>
            <td>
                <b>
                    FIR-9: Identity enhancements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly-fir/pull/9

@awrichar - the E2E is passing on these changes, but leaving PR in review state as I'd like to add some more E2E tests and do migration testing before pulling it out of draft.

I will put comments in-line in the code to help orient your review
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 21:57:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/548" class=".btn">#548</a>
            </td>
            <td>
                <b>
                    Rename contract subscriptions to contract listeners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes several noteworthy changes:

- Contract Subscriptions have now been renamed to Contract Listeners everywhere, to reduce confusion. This includes the `/contracts/subscriptions` endpoint. It is now `/contracts/listeners`
- The `/subscribe` endpoints on Contract Interfaces and APIs have been dropped
- The `/contracts/listeners` endpoint can now take a interface reference to point it at an existing FFI, rather than putting the full FFI for the event inline
- `blockchain_event` has been renamed to `blockchain_event_received`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 21:38:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/547" class=".btn">#547</a>
            </td>
            <td>
                <b>
                    [charts-by-type] histogram broken down by type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #546 

Support for histogram buckets that are grouped by `type`

Example Response:
```json
[
  {
    "buckets": [
      { "timestamp": "2022-02-23T22:40:33Z", "count": "23" },
      { "timestamp": "2022-02-23T22:45:33Z", "count": "0" },
      { "timestamp": "2022-02-23T22:50:33Z", "count": "14" }
    ],
    "type": "transaction_submitted"
  },
  {
    "buckets": [
      { "timestamp": "2022-02-23T22:40:33Z", "count": "16" },
      { "timestamp": "2022-02-23T22:45:33Z", "count": "0" },
      { "timestamp": "2022-02-23T22:50:33Z", "count": "14" }
    ],
    "type": "blockchain_event"
  },
  {
    "buckets": [
      { "timestamp": "2022-02-23T22:40:33Z", "count": "22" },
      { "timestamp": "2022-02-23T22:45:33Z", "count": "0" },
      { "timestamp": "2022-02-23T22:50:33Z", "count": "11" }
    ],
    "type": "message_confirmed"
  },
  {
    "buckets": [
      { "timestamp": "2022-02-23T22:40:33Z", "count": "1" },
      { "timestamp": "2022-02-23T22:45:33Z", "count": "0" },
      { "timestamp": "2022-02-23T22:50:33Z", "count": "1" }
    ],
    "type": "token_pool_confirmed"
  },
  {
    "buckets": [
      { "timestamp": "2022-02-23T22:40:33Z", "count": "6" },
      { "timestamp": "2022-02-23T22:45:33Z", "count": "0" },
      { "timestamp": "2022-02-23T22:50:33Z", "count": "4" }
    ],
    "type": "token_transfer_confirmed"
  }
]

```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 22:56:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/544" class=".btn">#544</a>
            </td>
            <td>
                <b>
                    [transfer-type-query] allow filtering by type on token transfers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Echelberger <eberger727@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 20:22:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/543" class=".btn">#543</a>
            </td>
            <td>
                <b>
                    Fix empty swagger URLs on contract API creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly/issues/539
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 16:37:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/542" class=".btn">#542</a>
            </td>
            <td>
                <b>
                    Change query method to POST for custom contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly/issues/540
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 15:59:35 +0000 UTC
    </div>
</div>

