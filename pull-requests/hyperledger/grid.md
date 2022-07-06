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
                PR <a href="https://github.com/hyperledger/grid/pull/1454" class=".btn">#1454</a>
            </td>
            <td>
                <b>
                    Fix clippy lint introduced in 1.62.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Backport-0-3</span><span class="chip">main</span>
            </td>
            <td>
                This makes several changes necessary to remove all Clippy lint warnings introduced in the 1.62.0 rust release. The two main changes are: 

1. Allowing unused lifetimes in Diesel macros. 
2. Remove unnecessary allocations made when appending to an existing string
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 20:40:22 +0000 UTC
    </div>
</div>

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

