---
layout: default
title: aries-rfcs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-rfcs
---

# aries-rfcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-rfcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/781" class=".btn">#781</a>
            </td>
            <td>
                <b>
                    using BTreeMap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `Use a HashMap when`:

You want to associate arbitrary keys with an arbitrary value.

You want a cache.

You want a map, with no extra functionality.

`Use a BTreeMap when`:

You're interested in what the smallest or largest key-value pair is.

You want to find the largest or smallest key that is smaller or larger than something.

You want to be able to get all of the entries in order on-demand.

You want a map sorted by its keys
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-15 11:06:01 +0000 UTC
    </div>
</div>

