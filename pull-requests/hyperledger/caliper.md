---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1184" class=".btn">#1184</a>
            </td>
            <td>
                <b>
                    Fix CompositeRateController class bug (#1181)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Rename old "roundConfig" references to the new "testMessage"
* Extend TestMessage class with some functions to allow modification by CompositeRateController
* Fix passed arguments to the new RateControl constructor when creating subcontrollers
* Add a composite rate controller to one of the Fabric CI phases

Fixes #1181 

Signed-off-by: Attila Klenik <a.klenik@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 23:17:26 +0000 UTC
    </div>
</div>

