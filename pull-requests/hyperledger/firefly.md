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
                PR <a href="https://github.com/hyperledger/firefly/pull/633" class=".btn">#633</a>
            </td>
            <td>
                <b>
                    Update batch manager dispatch to track inflight and fix private blobs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Batch manager updates

I believe I've found an issue in the way the batch manager and the batch processors interact
Because the messages stay in ready state while they are being dispatched, the `readPage` loop will still see all messages that are dispatched

Currently it attempts to re-dispatch them when it's told to rewinds, and relies on the processor to de-dup those messages
It all works from a consistency perspective, but with the pattern of workload from the long-run it's a little inefficient in terms of how many rewinds and re-processing we do. It seems this can reach the point the batch manager can get jammed up trying to do those re-dispatches to the processor, while the processor is busy flushing what it's got

This PR simplifies the logic significantly, by preventing duplicate dispatches in the batch manager.

The manager keeps a map of all in-flight dispatched sequences to processors, and the processors call back to the manager when they have flushed a batch (so the messages will no longer turn up in `readPage` queries).

### Fix to private blobs

The private message batch dispatcher, was only sending the first blob in a batch. Meaning other messages with blobs in the batch would never be confirmed, because the blobs never arrived.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-27 18:43:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/630" class=".btn">#630</a>
            </td>
            <td>
                <b>
                    Do not return an error from status if node lookup fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In `v0.14.0` if you register your org (only), and then call `/api/v1/status` you receive:

```js
{"error":"FF10277: Identity could not be resolved via DID 'did:firefly:node/zzhc7hdmc0'"}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 20:15:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/629" class=".btn">#629</a>
            </td>
            <td>
                <b>
                    [ui-v0.6.3] v0.6.3 release of ui in manifest
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
        Created At 2022-03-25 19:23:38 +0000 UTC
    </div>
</div>

