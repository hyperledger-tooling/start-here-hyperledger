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
                PR <a href="https://github.com/hyperledger/grid/pull/917" class=".btn">#917</a>
            </td>
            <td>
                <b>
                    Move workflow-aware permission check into SDK
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This removes the `check_permission_with_workflow` from the Purchase order smart contract's handler module to the SDK, as a method defined for the `PermissionChecker` in Pike. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-01 20:02:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/916" class=".btn">#916</a>
            </td>
            <td>
                <b>
                    Add GHA
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
        Created At 2021-09-01 14:16:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/915" class=".btn">#915</a>
            </td>
            <td>
                <b>
                    Add purchase order list and show functionality
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added purchase order list and show functionality in the CLI. This 
included updating the SDK client's fetch_entities_list to support 
multiple query string parameters via a hashmap, implementing list and 
show for purchase orders within ReqwestPurchaseOrderClient, and 
implementing the list and show functionality for the CLI.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-31 19:38:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/914" class=".btn">#914</a>
            </td>
            <td>
                <b>
                    Fix clippy error in CLI build file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes unneeded references from the CLI's `build.rs` file.
These references caused errors when running `just lint`.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-31 16:44:29 +0000 UTC
    </div>
</div>

