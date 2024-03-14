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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/335" class=".btn">#335</a>
            </td>
            <td>
                <b>
                    Upgrade the version of JUnit vintage gradle used
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Again for CVE-2020-15250.


testImplementation 'org.junit.vintage:junit-vintage-engine:5.3.1' imports `junit:junit:4.12`... gotta move to `org.junit.vintage:junit-vintage-engine:5.10.2` to get to `junit:junit:4.13.2`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 18:55:12 +0000 UTC
    </div>
</div>

