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
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    Provide a way for policy engines to pass additional state to callbacks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Provides an alternative approach the 2nd item in #91 , allowing any policy engine implementation to pass a closure in with additional variables it's safe for that implementation to pass through. For example, a transaction-specific context object.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 20:29:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    Expose filters for rich query
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - expose the filters for rich query tables so that they can be used externally.
- ~also updated the event handler callback function signatures to pass through the entire managed transactions so the other information (e.g. "from" field) becomes accessible.~
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 12:27:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/89" class=".btn">#89</a>
            </td>
            <td>
                <b>
                    Add suspend/resume transaction actions, and tweaks to history API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Adds `/suspend` and `/resume` `POST` actions to transactions
   - Uses the same approach as `DELETE` API
   - Response is `202` or `200` based on policy engine processing
- Disables compaction by default
    - It seems to add little value as policy engines usually are in cycles of multiple actions
    - It can get to the point the overhead is so high when 1000s of transactions are in flight with a 5min time window, and 100s of thousands of TX History entires per TX, that the transaction writer is overloaded and times out flushing `suspend`/`resume` actions in 30s.
- Does not include `history` array by default on transaction `GET` by ID
   - New `history` boolean option to return that value
- Renames the query parameter `count` for the `/history` API to `occurrences`
  - Avoid clash with the pagination option `count`
  - Does not change the JSON object to ensure backwards compatibility
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-30 17:58:30 +0000 UTC
    </div>
</div>

