---
layout: default
title: grid-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid-docs
---

# grid-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/333" class=".btn">#333</a>
            </td>
            <td>
                <b>
                    Add polling calls to DLT event monitor document
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The DLT event monitor document previously called for batch updates to
happen in real-time as they came in from the DLT stream. Unfortunately,
the current implementation of the DLT event stream does not include
sufficient information to allow a useful batch status update. This
change proposes an alternate solution: The DLT event monitor uses events
as a cue that a batch was updated. It then calls out to the polling
monitor, which gathers the associated batch information.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-03 19:45:41 +0000 UTC
    </div>
</div>

