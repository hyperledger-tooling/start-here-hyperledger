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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/998" class=".btn">#998</a>
            </td>
            <td>
                <b>
                    asset-transfer-basic CI improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Application failure should result in CI failure (exit code 1)
- Automatically remove wallet from prior runs 
- Fix chaincode name issues, allow chaincode name to be passed from CI
- Fix appUser collisions (duplicate registration failures)
- Fix key create collisions across apps (in cases where same chaincode is used for multiple apps)

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 21:38:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/996" class=".btn">#996</a>
            </td>
            <td>
                <b>
                    Update Go and Go dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update go dependencies in sample chaincodes and applications.
Update Go to 1.19.6

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 22:05:16 +0000 UTC
    </div>
</div>

