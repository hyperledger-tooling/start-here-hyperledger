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
                PR <a href="https://github.com/hyperledger/grid/pull/1420" class=".btn">#1420</a>
            </td>
            <td>
                <b>
                    Add submission struct
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                Adds the struct that represents a batch submission. This will be used by
the future submitter and queuer components.

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 22:04:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1419" class=".btn">#1419</a>
            </td>
            <td>
                <b>
                    Use actix-rt library for testing actix async
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                Switch from tokio to actix-rt for actix async tests so the versions
don't clash with tokio's version.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 21:25:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1416" class=".btn">#1416</a>
            </td>
            <td>
                <b>
                    Add REST API batch submission handler trait
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This adds a trait for a component of the REST API that submits batches. It will take in a generic bytes representation of the batch to be submitted (or batch list) and other information pertaining to the batch to be persisted by Grid. This will be used by endpoints that accept batches, in order to process generic `TransactionPayload`s to store them as batches in Grid's DB, or to send them to an upstream server for further handling. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 22:21:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1415" class=".btn">#1415</a>
            </td>
            <td>
                <b>
                    Add `batch_submission` mod and `url_resolver`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                Adds the url_resolver submitter subcomponent and the batch_submission
module structure that contains it.

Resolves: #1414

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 16:19:39 +0000 UTC
    </div>
</div>

