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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1450" class=".btn">#1450</a>
            </td>
            <td>
                <b>
                    Add config object for Griddle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Epic: Griddle</span><span class="chip">main</span>
            </td>
            <td>
                This change adds a 'config' module to Griddle (currently unused) that will be utilized to build the Griddle daemon to run. This allows for config values to be collected from various sources, currently including environment vars, default values, and clap arguments. 

TODO: 
- Actually, I need to update some tests still. There are over-arching tests for the `GriddleConfig` object using the various partial config objects that should be completed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 15:37:33 +0000 UTC
    </div>
</div>

