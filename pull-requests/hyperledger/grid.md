---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1398" class=".btn">#1398</a>
            </td>
            <td>
                <b>
                    Add `clean_stale_records` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This adds an operation to clean batch tracking records that were created
    before a specified time. This works by removing batch records with a
    `created_at` value less than the specified timestamp. As the other
    batch tracking tables all use foreign keys derived from the batch_id and
    that use cascading deletes, this will remove the batch record and any
    associated "child" records.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 20:44:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1393" class=".btn">#1393</a>
            </td>
            <td>
                <b>
                    Add `get_failed_batches` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This adds an operation to get failed batches. This also adds a unit test for the operation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 19:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1392" class=".btn">#1392</a>
            </td>
            <td>
                <b>
                    Upgrade reqwest version to 0.11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                0.11 removes an unnecessary trait bound on the post method that we would
otherwise need to implement in the upcoming submitted component.

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 16:30:17 +0000 UTC
    </div>
</div>

