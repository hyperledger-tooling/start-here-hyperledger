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
                PR <a href="https://github.com/hyperledger/grid/pull/1432" class=".btn">#1432</a>
            </td>
            <td>
                <b>
                    Update `/batches` endpoint to correctly return errors from Splinter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                This PR closes #1430 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 20:17:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1431" class=".btn">#1431</a>
            </td>
            <td>
                <b>
                    Remove slack alerts from pull request workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These were introduced inadvertently as a copy/paste error. Not only would
this behavior be undesired, but because the workflow runs in the context
of the forked repository there is no access to the secrets required.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 19:53:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1429" class=".btn">#1429</a>
            </td>
            <td>
                <b>
                    Retire chenette and eloaverona
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This change retires @chenette and @eloaverona as maintainers and
codeowners for Grid.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 14:46:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1428" class=".btn">#1428</a>
            </td>
            <td>
                <b>
                    Make Chris Eckhardt a Grid maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 13:50:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1427" class=".btn">#1427</a>
            </td>
            <td>
                <b>
                    Add `TrackingBatchResourceBuilder` for constructing batches from generic transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This change adds a struct, `TrackingBatchResourceBuilder`, that will be used by endpoints to construct a batch from a generic list of transactions. This struct also takes identifying information for the batch, including the service ID, any data change IDs, and the signer's public key. 

This struct is serializable/deserializable, as it will be used to pass batches across the API to be persisted in Grid's database.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 13:47:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1425" class=".btn">#1425</a>
            </td>
            <td>
                <b>
                    Update Grid to use `actix_web` 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This updates grid to use `actix_web` v4. Both v3 and 4 cannot be supported in Grid due to conflicting re-exports of tokio structs/traits from the libraries. Therefore, all rest api code and tests in the Grid SDK, Griddle, and the Grid Daemon is updated to use actix_web 4.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 19:16:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1424" class=".btn">#1424</a>
            </td>
            <td>
                <b>
                    Add submitter and observer traits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                Adds the public traits for the submitter and submitter observer. These will be used in future implementations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 16:27:47 +0000 UTC
    </div>
</div>

