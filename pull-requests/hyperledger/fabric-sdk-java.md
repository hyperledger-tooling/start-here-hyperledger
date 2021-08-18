---
layout: default
title: fabric-sdk-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-java
---

# fabric-sdk-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    Explicit dependencies in integration test chaincode (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of fc05ef2accde5956ce930623d11d5443a4d759cf from main branch.

Resolves breakages with latest releases of the chaincode shim, where more recent Gradle versions are more strict in requiring dependencies to be specified rather than picked up as transient dependencies.

Also update commons-compress dependency to address security vulnerability.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 15:50:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/143" class=".btn">#143</a>
            </td>
            <td>
                <b>
                    Explicit dependencies in integration test chaincode
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
        Created At 2021-08-18 08:39:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/142" class=".btn">#142</a>
            </td>
            <td>
                <b>
                    Update Chaincode Dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Set the chaincode dependency to be 2.2.+ so that it uses the latest LTS release.
2.+ will pull in any development version beta etc...

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 07:35:38 +0000 UTC
    </div>
</div>

