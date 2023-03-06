---
layout: default
title: fabric-admin-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-admin-sdk
---

# fabric-admin-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-admin-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    Update godoc and examples for chaincode package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Made the Definition.validat() function private since it is not used outside of the package.

Closes #101 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 17:22:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    Implement GetInstalled chaincode package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contains two commits to be merged as separate commits. One for GetInstalled chaincode package; the other for QueryApproved chaincode definition.

Changed chaincode.PackageID() to take a Reader for consistency with chaincode.Install().

Closes #102
Closes #103
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 17:40:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    try to fix #106
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I suppose we need to provide function to support approve sign for chaincode level and channel level.
this PR is just a draft as POC.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 15:21:35 +0000 UTC
    </div>
</div>

