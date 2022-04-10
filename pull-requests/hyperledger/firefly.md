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
                PR <a href="https://github.com/hyperledger/firefly/pull/665" class=".btn">#665</a>
            </td>
            <td>
                <b>
                    Add rewinder to handle enrichment off event poller critical path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Issue #663 demonstrated that the event loops of the various plugins cannot safely ask the DB for information the event aggregator loop is updating, concurrently to the event poller writing it.

However, we don't want to slow the event poller down by making it do complex enrichment tasks to work out how to rewind. These tasks are as follows:
- For blobs: Query all `data` IDs associated with a `blob` hash, then find all `message` IDs that are associated with that data
- For token transfers: Query the `batch` ID associated with the message, which is associated with the on-chain transfer

So this PR introduces the architecture summarized in the diagram below. This ensures we do **not** start the enrichment DB activities (in loop 2) until the event poller has completed the cycle that might have been active while the plugin event that generated the rewind was active

![pr_665_diagram_1](https://user-images.githubusercontent.com/6660217/161826863-3c4dc41b-03a0-444a-a851-cf476e6f22d5.jpg)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 18:37:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/662" class=".btn">#662</a>
            </td>
            <td>
                <b>
                    Proper handling of token approval events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Ensure existing approvals are not being overwritten
- Remove localID from async/sync POST response
- Commented out approvals from synchronous tokens e2e test due to https://github.com/hyperledger/firefly/issues/661
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 20:08:52 +0000 UTC
    </div>
</div>

