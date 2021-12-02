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

