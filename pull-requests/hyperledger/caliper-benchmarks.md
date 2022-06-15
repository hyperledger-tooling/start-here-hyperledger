---
layout: default
title: caliper-benchmarks
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper-benchmarks
---

# caliper-benchmarks <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper-benchmarks){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/204" class=".btn">#204</a>
            </td>
            <td>
                <b>
                    Add support for a composite read/write transaction to fixed asset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #201 

Addresses all points and features of #201 except for random writing of keys. You have to choose if either writes to keys that were already read or not.
I would outline that if you want to only write to already read keys you need to make sure that the number of read keys is equal to or more than the number of write keys; if not you only part (as much as the number of read keys you have) of already read keys and the rest would be new ones.

One possible improvement to the benchmark file could be to automatically derive a number of assets to initialize from the total number of tx multiplied by the read+write transaction instead of having to input it manually in the round definition options.

Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 15:37:18 +0000 UTC
    </div>
</div>

