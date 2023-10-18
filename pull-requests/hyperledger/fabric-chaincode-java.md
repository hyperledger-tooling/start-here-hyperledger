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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/317" class=".btn">#317</a>
            </td>
            <td>
                <b>
                    Move to Gradle v7.6.3 for all wrappers.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As per https://nvd.nist.gov/vuln/detail/CVE-2023-44387, Gradle v7.6.2 is vulnerable.  Moves all incorporate wrappers to the latest version of Gradle in their properties spec such that they use the latest Gradle (on the 7.6.x branch) to run the build.

Related to https://github.com/hyperledger/fabric-chaincode-java/issues/312 but not mentioned explicitly in that issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 21:28:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/316" class=".btn">#316</a>
            </td>
            <td>
                <b>
                    Move to org.json:json 20231013.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As per https://github.com/hyperledger/fabric-chaincode-java/issues/312, and also per https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-5072, the newest version of org.json:json should be used.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 20:54:33 +0000 UTC
    </div>
</div>

