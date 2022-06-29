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
                PR <a href="https://github.com/hyperledger/grid/pull/1453" class=".btn">#1453</a>
            </td>
            <td>
                <b>
                    Add dlt polling monitor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                This change adds the dlt polling monitor base module to Grid as an
experimental feature.

Signed-off-by: Amelia Bradley <bradley@bitwise.io>

Some notes on things that need to be completed
- [ ] Split into multiple files (runnable / running)
- [ ] Add shutdown on process shutdown message
- [ ] Add timing component with tokio

This uses traits for any interactions with the REST API or the DB, which are part of separate tasks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 14:19:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1452" class=".btn">#1452</a>
            </td>
            <td>
                <b>
                    Clean up unused imports in scope_id tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 22:37:34 +0000 UTC
    </div>
</div>

