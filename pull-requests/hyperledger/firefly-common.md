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

