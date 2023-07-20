---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    Add field selection on GetMany and tweaks to Filter API builder pattern
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Support field-level selection/redaction in `CRUD` only
   - Adds to base `Filter` library
   - Implements in `CRUD` helper
   - Adds to API/Swagger _only if_ `SupportFieldRedaction` is set
       - This is because FireFly Core is not using `CRUD` library and hence will not support this
- Convenience of having modifiers on the base `FilterBuilder` so you can do:
    ```go
    fb.And(conditions...).Limit(1).Sort("-created") // possible before: results in Filter
    fb.Limit(1).Sort("-created").And(conditions...) // now possible: results in AndFilter
    ```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-17 19:40:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/90" class=".btn">#90</a>
            </td>
            <td>
                <b>
                    convert int value unset log to trace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As described in the title, I'm using the behaviour of getting the 0 big.Int back when the string is empty, it starts to become annoying to see this log line at debug level.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-17 12:45:59 +0000 UTC
    </div>
</div>

