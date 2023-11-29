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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    Fix docs regression in parameter descriptions that changes swagger gen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We're incorrectly adding a `[0]` to these messages after #107:

```
description: 'The maximum number of records to return (max: [0])'
                                                            ^^^
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 16:26:32 +0000 UTC
    </div>
</div>

