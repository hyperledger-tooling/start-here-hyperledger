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

