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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/394" class=".btn">#394</a>
            </td>
            <td>
                <b>
                    Several small fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is more of an appropriate size for @bvavala with several small fixes. It should be independent of the makefiles PR (meaning that they should be able to be applied in either order). 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-25 22:49:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/392" class=".btn">#392</a>
            </td>
            <td>
                <b>
                    Clean up a bunch of the Makefiles and dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                First, this removes a lot of extraneous (and sometimes just wrong definitions from the Makefiles and CMakefiles.

Second, this adds a custom command for the pservice and eservice that creates a header file with the MRENCLAVE for each of the enclave libraries. This include file can be used by any application that needs to verify the enclave. For example CCF TP should be using the file.

Finally, this brings a little more consistency to the use of activate and python in the Makefiles. There is no need to activate the virtual environment prior to building one of the components.

Signed-off-by: Mic Bowman <mic.bowman@intel.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-20 00:47:03 +0000 UTC
    </div>
</div>

