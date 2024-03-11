---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6678" class=".btn">#6678</a>
            </td>
            <td>
                <b>
                    Bugfix - only track intrinsically bad blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This is a follow-up to PR https://github.com/hyperledger/besu/pull/6622.  Rework bad block handling so that we are only tracking blocks that are intrinsically bad due to a spec-related validation error.  We should not be marking blocks as bad if we are missing data locally or encounter some unspecified exception during block processing.  

## Fixed Issue(s)
Tangentially related to https://github.com/hyperledger/besu/issues/6301

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 22:07:39 +0000 UTC
    </div>
</div>

