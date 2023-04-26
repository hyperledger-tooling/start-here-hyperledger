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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/66" class=".btn">#66</a>
            </td>
            <td>
                <b>
                    Cache utility needs namespace grouping and reset capability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Existing consumers of caches (core in particular) require the ability to group caches together under a `namespace`, using the same name in different namespaces.

Then the ability to clear all caches that are in the same namespaces.

Consumers that don't need that function can simply specify an empty string for namespace (as it's possible to have multiple different managers as well).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 16:12:09 +0000 UTC
    </div>
</div>

