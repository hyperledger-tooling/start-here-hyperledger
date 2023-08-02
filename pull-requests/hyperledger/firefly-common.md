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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    Convenience function for dynamic scoping, and fix to filtering in StringFieldLower
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 16:10:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    Add optional name/get-first semantics to CRUD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's common (including in FireFly core) to have:
- A special `name` column, that can be used in paths as an alternative to UUID
- To have IDs that must conform to a special syntax - especially UUIDs
- To want to do a get that returns zero/one entry for some filter combination that is not the ID

This PR provides those features as optional base functionality in `CRUD` to avoid the need to implement many times.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 15:19:36 +0000 UTC
    </div>
</div>

