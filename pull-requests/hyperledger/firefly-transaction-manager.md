---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Restructure TX input for consistency with ethconnect and idempotence
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ... also removes the last vestige of a dependency on FF Core 🪶 

I've merged #15 into this branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 22:11:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Add support for deploying contracts
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
        Created At 2022-08-02 18:36:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    Ensure consistent block state during cycle, to prevent out-of-order delivery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I realized that there was a gap in the ordering logic, in the case that there is a number of pending event waiting confirmation and we go through and do `walkChain()`.

Specifically if new blocks become available during that cycle, we might get a "hit" for a block for a later event, which was a "miss" for that block for an earlier event - simply because the block has just been mined.

So I've added a `blockState` that is created each time we do a cycle, that ensures we don't change answers on ourselves for the duration of that cycle.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 13:07:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/14" class=".btn">#14</a>
            </td>
            <td>
                <b>
                    Flatten event delivery JSON payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The JSON payload expected by FireFly (established by ethconnect) requires top-level fields for all the `info` content - both that which is mandated by the FFTM framework, and that which is extensible in the connector.

This took a bit of faff to sort out, as Go doesn't have a trivial mechanism to merge custom fields into a structure with declared fields. So there's a utility function added (which could move to `common` in the future) to help with that merging, and a new custom `Unmarshal`/`Marshal` function on the `EventWithContext` struct - which also moved to `apitypes`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 12:45:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Events fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds some fixes for event and receipt delivery over websockets.

### Tested and working:
🟢 Event delivery with 0 required confirmations and on demand mining (standard E2E test configuration)
🟢 Event delivery with 2 required confirmations and 2 second block period

### Tested and sometimes working:
🟡 Receipt delivery over WebSocket with 0 required confirmations and on demand mining (standard E2E test configuration). More details below.

### Tested and not working:
🔴 Receipt delivery over WebSocket with 2 required confirmations and 2 second block period. More details below

### Open questions
- Where is the right place in the code to send the WebSocket message when we have a transaction receipt to deliver? It's currently in the `receiptCallback` function in `policyLoop.go` but it's part of a `manager`. Feels like it might be the right code, but maybe the wrong file?
- I don't think I have the code quite right to handle when a transaction is "done" and confirmed. There are several states a transaction can be in, and I don't think that concept used to exist in the previous ethconnect receipt model.

### Known issues
- When required confirmations is set to `0` and using on demand mining, occasionally (seems like when I send several transactions in quick succession) it will log something like:
```
[2022-07-28T12:58:04.695-04:00] DEBUG evmconnect: Receipt for transaction 0xeb84df74d0354b91b696cf4f964e58fbf6b9f25e0df0a95186b5c1fda83bd616 not yet available
```
There is a comment at the end of that function which says:
```
// No need to keep polling - either we now have a receipt, or normal block header monitoring will pick this one up
```
However it appears that the receipt is not picked up by the normal block header monitoring, or for some reason its receipt callback function is not called. This is the yellow bullet point above.

- When required confirmations is set to `2` and using a 2 second block period, it looks like the receipt callback is never called at this point.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 14:28:41 +0000 UTC
    </div>
</div>

