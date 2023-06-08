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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/71" class=".btn">#71</a>
            </td>
            <td>
                <b>
                    Allow any string for ID column, and support collections without an `updated` column
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Couple of constraints that while working on FFTM/EVMConnect I found were unnecessary.

1. Allowing any string for ID
  - The default example `ResourceBase` still uses fftypes.UUID
  - This allows FFTM to use the `namesace:UUID` convention from FF Core (established historically)
2. Allowing collections without an `updated` column
  - The previous code allowed you to map the `created`/`updated` columns to any fields in your business object, but required them. This was a pain for write-or-delete-only data, which is true for performance sensitive transaction history records in FFTM/EVMConnect
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 02:20:31 +0000 UTC
    </div>
</div>

