---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/533" class=".btn">#533</a>
            </td>
            <td>
                <b>
                    Use chaincode action response payload as transaction result
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The top-level response payload in the proposal response is not required to contain the transaction result and may be used to hold metadata. Even though current Fabric implementations typically duplicate the transaction result in the top-level response payload, this actually causes failures due to message size limits in some cases, so might change and should not be relied upon.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 17:47:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/532" class=".btn">#532</a>
            </td>
            <td>
                <b>
                    Issue 508
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
        Created At 2021-11-18 08:18:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/531" class=".btn">#531</a>
            </td>
            <td>
                <b>
                    Remove mkdocs.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                mkdocs.yaml is not used and the content within is outdated and not correct.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 11:16:52 +0000 UTC
    </div>
</div>

