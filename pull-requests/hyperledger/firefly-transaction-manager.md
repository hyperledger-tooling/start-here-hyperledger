---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    Fix bug that causes history summary to grow incorrectly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a unit test to recreate the bug and flag up regressions in the future.

Signed-off-by: Matthew Whitehead <matthew1001@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 19:42:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/58" class=".btn">#58</a>
            </td>
            <td>
                <b>
                    Suggestions on TODOs and comments/naming for TX History API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @matthew1001 - this is the promised PR review / TODO help from PR #51, covering my high level comments.

I'm afraid I didn't get to looking at the reason you're seeing out-of-order serialization on some paths.

The items I've tried to provide here are:
- Simplifying config to one parameter
    - I believe only one array needs a limit, the others are limited by the list of different types
- Passing config to the TX History API
    - I refactored it out to a separate `txhistory.Manager` instanced, and added that into what's passed to the Policy Engine
    - I called this new structure `policyengine.ToolkitAPI` which I think is in-line with the evolving architecture
- Comments / code naming / removing fields
    - I've added code comments with my understanding of the intent of the different sections, both to validate my current understanding, and to aid future developers of policy engines.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 19:26:34 +0000 UTC
    </div>
</div>

