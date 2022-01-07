---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    Add GHA for publishing tagged releases to crates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 21:35:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    Alter column type for leaf address
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prior to this change, the column type for merkle_radix_leaf.address was specified as `"STRING"`. As this type is not one of the types automatically treated as `TEXT`, it defaults to being treated as a `NUMERIC` value.  With certain addresses, where all characters were valid decimal digits with a leading zero, the leading zero would be dropped. This would create
instances where the address value would not be returned, but not with the same address queried.

Changing the column type to `"TEXT"` fixes the problem.

The migration added will also correct all address that are missing a leading zero.

This change also adds several tests for both SQLite and Postgres to guard against this issue in the future, while also exercising the `list_leaves` trait function implementations of each.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 17:04:50 +0000 UTC
    </div>
</div>

