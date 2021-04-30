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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/653" class=".btn">#653</a>
            </td>
            <td>
                <b>
                    Update Grid Logo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the Grid logo used by the Grid UI. This version has a white
background instead of a transparent one.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 17:02:07 +0000 UTC
    </div>
</div>

