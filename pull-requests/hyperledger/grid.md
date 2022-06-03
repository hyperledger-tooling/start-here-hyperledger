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
                PR <a href="https://github.com/hyperledger/grid/pull/1439" class=".btn">#1439</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-3: Test grid-ui docker build in CI 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0-3</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-03 00:20:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1438" class=".btn">#1438</a>
            </td>
            <td>
                <b>
                    Test grid-ui docker build in CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Backport-0-3</span><span class="chip">main</span>
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 21:36:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1437" class=".btn">#1437</a>
            </td>
            <td>
                <b>
                    Add release notes for v0.3.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0-3</span>
            </td>
            <td>
                Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 14:42:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1436" class=".btn">#1436</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-3: Update `/batches` endpoint to correctly return errors from Splinter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of: https://github.com/hyperledger/grid/pull/1432
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 14:31:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1435" class=".btn">#1435</a>
            </td>
            <td>
                <b>
                    Update Grid rest api to use actix web 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                This updates the rest api code in Grid's SDK, Griddle, and the Grid
Daemon to use Actix Web 4. This replaces actix web 3 in this codebase as
both versions can't be supported due to conflicting re-exports of tokio
structs/traits.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-31 15:57:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1434" class=".btn">#1434</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-2: Remove slack alerts from pull request workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0-2</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-27 20:47:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1433" class=".btn">#1433</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-3: Remove slack alerts from pull request workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0-3</span>
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
        Created At 2022-05-27 20:47:13 +0000 UTC
    </div>
</div>

