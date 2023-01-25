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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/393" class=".btn">#393</a>
            </td>
            <td>
                <b>
                    miscellaneous fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains some random (small) fixes. It currently includes all the build changes so do not merge. If these changes look fine, it can pull them out so it can be applied separately (without the bigger makefile changes).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-25 15:54:15 +0000 UTC
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

