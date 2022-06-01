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
                <span class="chip">Backport-0-3</span><span class="chip">main</span>
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

