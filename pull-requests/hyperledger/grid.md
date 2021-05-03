---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/660" class=".btn">#660</a>
            </td>
            <td>
                <b>
                    Remove unsupported Memory Store impls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This removes now-unsupported MemoryStore implementations for the
commits and schemas stores. The memory store implementations were
deprecated in favor of an in-memory sqlite implementation but it looks
like a couple of the modules' implementations didn't get cleaned up.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 16:36:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/659" class=".btn">#659</a>
            </td>
            <td>
                <b>
                    Replace specific store errors with standard ones
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This replaces the StoreFactoryCreationError and ParseConnectionUriErrors
with the standard Grid InternalError type. This is more in line with the
approach used across the rest of the SDK.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 16:29:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/658" class=".btn">#658</a>
            </td>
            <td>
                <b>
                    Make all operations atomic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This makes all operations atomic. Previously, this was done in a sort of
piecemeal fashion. This just cleans this up and makes sure all
operations are wrapped in the generic diesel transaction. This is
available for all Diesel backends that implement Diesel::Connection.
This depends on PR #656.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 16:27:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/657" class=".btn">#657</a>
            </td>
            <td>
                <b>
                    Update PurchaseOrderStore feature guard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the DieselPurchaseOrderStore feature to be guarded by the
`diesel` feature rather than the `postgres` feature. This brings the
module in line with the other Grid data stores. This is part of stabilizing the
postgres and sqlite features.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 16:23:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/656" class=".btn">#656</a>
            </td>
            <td>
                <b>
                    Rename `fetch_` operations to `get_`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This renames the `fetch_` operations to `get_` operations. This brings
the Grid data store operation in line with the naming conventions used
in Splinter. This is part of stabilizing the postgres and sqlite features.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 16:19:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/655" class=".btn">#655</a>
            </td>
            <td>
                <b>
                    Add date created field to rest api resources
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds database generated date create timestamp to agent, role, organization, product, location, and schema endpoints.

Example:

```
GET /agent/021bab739fce4133204c8c0bd939d48e4d32e5b29eb87ed871d2666fcd3f51bb3e
{
  "public_key": "021bab739fce4133204c8c0bd939d48e4d32e5b29eb87ed871d2666fcd3f51bb3e",
  "org_id": "crg",
  "active": true,
  "roles": [
    "admin"
  ],
  "metadata": {},
  "date_created": 1619707637
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 21:05:57 +0000 UTC
    </div>
</div>

