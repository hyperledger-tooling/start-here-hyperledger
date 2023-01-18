---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/391" class=".btn">#391</a>
            </td>
            <td>
                <b>
                    Fix build in HW mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes an issue in the build in HW mode.

The issue is due to missing target dependencies in the pservice build.
When the `build` target triggers the cmake, the `contract_enclave_mrenclave.cpp` file (part of the `ENCLAVE_FILES` target) must be available, as the cmake checks for that.
However, there is no dependency between the two targets.

Curiously, this issue seems to have been uncovered by unintentionally making the build single-task.
So far, apparently, the `make all` triggered both targets in parallel in the right order.

Signed-off-by: Bruno Vavala <bruno.vavala@intel.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 01:04:02 +0000 UTC
    </div>
</div>

