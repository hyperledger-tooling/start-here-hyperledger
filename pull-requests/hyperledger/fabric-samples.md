---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/909" class=".btn">#909</a>
            </td>
            <td>
                <b>
                    Run FSAT tests with 2.5 images, binaries, and trigger on all builds for regression coverage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR runs the FSAT tests for all commits, not just edits under the full-stack-asset-transfer guide sub-folder.

We had some regressions in the fabric-shim when moving to 2.5.1 which would have been caught by the FSAT tests, had they been run with all of the samples commits.  This PR re-enables the FSAT tests to run on all builds: 

- runs with 2.5 binaries/ images 
- pins fabric-contract-api and fabric-shim to 2.4.0 (still some issues to sort out with 2.5.1) 
- Removes an annoying lint warning for unused variables.
- Displays a useful message to the console, explaining why Bananaman can not transfer a token to Appleman.   (In some cases of users running through the workshop, it was not clear that there was work to be done to implement this one-line function.)

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 16:15:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/908" class=".btn">#908</a>
            </td>
            <td>
                <b>
                    Swap to use the Helper Function to create policies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The old way used the direct protobuf functions, there is a helper function in the chaincode does exactly that.

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 09:51:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/907" class=".btn">#907</a>
            </td>
            <td>
                <b>
                    Swap to use the Helper Function to create policies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The old way used the direct protobuf functions, there is a helper function in the chaincode does exactly that.

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 09:49:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/906" class=".btn">#906</a>
            </td>
            <td>
                <b>
                    run test suites with 2.5 binaries and images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Runs the fabric-samples test suites with Fabric 2.5 images and binaries.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 20:01:21 +0000 UTC
    </div>
</div>

