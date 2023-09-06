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
                PR <a href="https://github.com/hyperledger/firefly/pull/1398" class=".btn">#1398</a>
            </td>
            <td>
                <b>
                    Do not expect to retrieve local org during definition handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                Only the org DID is needed for this check - no need to actually look up the org from the database. At this point the message author has already been verified, so a database lookup here is just extra unnecessary processing (and can lead to infinite retries if it fails).

Fixes #1397
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 18:47:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1396" class=".btn">#1396</a>
            </td>
            <td>
                <b>
                    Proposal: Generic subscription options while adding contract listener
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Generic subscription options while adding contract listener

Generic options for the automatically generated subscription can be passed in listener options

```json
{
  "name": "PayPerUseListener",
  "options": {
    "firstEvent": "newest",
    "subscriptionOptions": {
      "additionalOption1": "option1",
      "additionalOption2": "option 2"
    }
  },
  "topic": "default1"
}
```

## Intention

A privacyGroupId could be passed to Ethconnect and calls to priv_getLogs etc. would be possible.
Every plugin would be able to listen for the subscriptionOptions necessary for its subscription configuration.

The introduced changes do not break existing functionality.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 14:19:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1395" class=".btn">#1395</a>
            </td>
            <td>
                <b>
                    handle update for unpublished API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update to unpublished contract APIs are no longer possible due to https://github.com/hyperledger/firefly/pull/1322

This PR fixes the problem by adding the upsert logic back in for unpublished contract APIs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 13:31:07 +0000 UTC
    </div>
</div>

