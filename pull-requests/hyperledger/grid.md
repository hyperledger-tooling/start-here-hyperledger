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

Resolves: #1141
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1164" class=".btn">#1164</a>
            </td>
            <td>
                <b>
                    Fix linting issues from rust 1.57
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes linting issues introduced in Rust 1.57
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 23:49:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1163" class=".btn">#1163</a>
            </td>
            <td>
                <b>
                    Stabilize `data-validation`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stabilize the data-validation feature for validating XML data by moving
it under stable

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 22:02:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1162" class=".btn">#1162</a>
            </td>
            <td>
                <b>
                    fix internal errs
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
        Created At 2021-12-02 19:09:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1160" class=".btn">#1160</a>
            </td>
            <td>
                <b>
                    Add po::partner permissions to po subworkflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds permissions for the "po::partner" permission alias.
This allows the partner permission alias to create and update a po
within the collaborative subworkflow. Previously, only the "po::buyer"
and "po::seller" had permissions to create and update a purchase order.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 17:05:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1159" class=".btn">#1159</a>
            </td>
            <td>
                <b>
                    Update po version create and update commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the `grid po version create` and `grid po version update`
cli commands to take the po number as the first positional argument
rather than a required flag. This seems more natural and is the pattern
used for the list and show version commands.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 16:33:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1158" class=".btn">#1158</a>
            </td>
            <td>
                <b>
                    Use as_ptr method for clarity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the drop implementations to use the as_ptr method instead of
self.0 for clarity.

Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 16:26:24 +0000 UTC
    </div>
</div>

