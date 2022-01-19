---
layout: default
title: fabric-chaincode-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-java
---

# fabric-chaincode-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/223" class=".btn">#223</a>
            </td>
            <td>
                <b>
                    Update build.gradle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move to recent log4j

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 19:29:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/222" class=".btn">#222</a>
            </td>
            <td>
                <b>
                    Improve the handling of the TLS certifiactes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For reasons lost in history, Fabric hasn't standised on whether to load certs in base64 or
PEM format. What does seem to be standard is if the environment variable ends in FILE then
it's a PEM format, but if it's PATH then it's base64.

This change will allow either FILE or PATH environment variables to be used in all cases.

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-12 09:47:54 +0000 UTC
    </div>
</div>

