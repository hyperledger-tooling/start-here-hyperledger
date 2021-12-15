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
                PR <a href="https://github.com/hyperledger/grid/pull/1182" class=".btn">#1182</a>
            </td>
            <td>
                <b>
                    v0.2 Rust 1.57 clippy updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 Rust 1.57 clippy updates for the 0-2 branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 15:27:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1181" class=".btn">#1181</a>
            </td>
            <td>
                <b>
                    Backport: Stabilize `cylinder-jwt-support` to 0-2 branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This includes the commit used to stabilize the `cylinder-jwt-support` feature in both the SDK and the daemon.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 22:31:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1180" class=".btn">#1180</a>
            </td>
            <td>
                <b>
                    Add tests for the purchase order endpoints provided by the daemon
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Mainly, this PR is a response to a request made in the stabilization process for the Grid Daemon's `purchase-order` feature. This PR adds tests to the purchase-order-specific rest endpoints. This also adds a field to the return objects, `service_id`, as this field allows for more thorough testing and is info that some clients may want or need.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 22:22:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1178" class=".btn">#1178</a>
            </td>
            <td>
                <b>
                    Add guard against multiple accepted po versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a check when updating po versions to "accepted" to ensure
there is not already an accepted version. Previously, users could
create multiple accepted versions.

Resolves: #1171

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 00:20:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1177" class=".btn">#1177</a>
            </td>
            <td>
                <b>
                    Simplify po cli batch actions and add tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The purchase order batch action functions all contained the same logic.
This change consolidates that logic into two functions, and adds a test
to verify that it acts as expected.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 23:21:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1176" class=".btn">#1176</a>
            </td>
            <td>
                <b>
                    Fix filter in po version query
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes a query filter in list_purchase_order_versions that allows
filtering based on accepted/not_accepted state. Previously,
filtering had no effect.

Required to fix issue #1171

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 20:56:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1175" class=".btn">#1175</a>
            </td>
            <td>
                <b>
                    Add doc comments to purchase_order rest api code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds doc comments to the structs in the purchase order rest api
code. This also adds doc comments to the functions in the same module.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 20:21:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1174" class=".btn">#1174</a>
            </td>
            <td>
                <b>
                    `purchase-order` SDK feature stabilization work
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes several updates to the SDK code guarded by the `purchase-order` feature. These changes were requested during the first round of stabilization reviews.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 19:24:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1173" class=".btn">#1173</a>
            </td>
            <td>
                <b>
                    Stabilization fixes for the `purchase-order` endpoints feature 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds module-level documentation and doc comments for any
public implementation. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 18:54:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1172" class=".btn">#1172</a>
            </td>
            <td>
                <b>
                    Stabilization updates for `workflow`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a few more stabilization updates, including beefed up module lvl and rustdoc comments and an update to the `can_transition` method.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 18:45:31 +0000 UTC
    </div>
</div>

