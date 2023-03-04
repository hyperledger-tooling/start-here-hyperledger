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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Add getter for DB provider features struct field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Looking into issue https://github.com/hyperledger/firefly/issues/1196 (now spun out into https://github.com/hyperledger/firefly/issues/1199) it appears that the `features` struct field is no longer visible to users of the package. Adding a getter in a similar way to the existing `ConnLimit()` getter makes the field accessible to read.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 15:24:24 +0000 UTC
    </div>
</div>

