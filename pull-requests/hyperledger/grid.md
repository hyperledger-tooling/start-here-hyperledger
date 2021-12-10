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

The previous implementation was likely being affected by another
existing bug, but this implementation is also simpler.

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
                    Add documentation to purchase order endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds module-level documentation and doc comments for any
public implementation.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1168" class=".btn">#1168</a>
            </td>
            <td>
                <b>
                    Stabilize `client-reqwest` feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This stabilizes the `client-reqwest` feature by moving it into "stable"
in the sdk/Cargo.toml file.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 20:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1167" class=".btn">#1167</a>
            </td>
            <td>
                <b>
                    Fix mislabeled workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Corrects an accepted workflow being built as a proposed workflow.

Resolves: #1156

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 20:20:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1166" class=".btn">#1166</a>
            </td>
            <td>
                <b>
                    Add xsd files to docker images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds product and purchase order xsd files to default locations so users running through the examples can create products and purchase order versions. Previously, users would have to copy the files from the Grid directory into the running container and in the correct location.

Resolves: #1141, #1155
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 17:46:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1165" class=".btn">#1165</a>
            </td>
            <td>
                <b>
                    Fix alternate ID bugs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes a couple bugs related to alternate IDs for purchase orders. There were two separate bugs that affected the ability to update the alternate IDs for a purchase order. One bug prevented adding new IDs and one prevented properly removing IDs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 16:35:08 +0000 UTC
    </div>
</div>

