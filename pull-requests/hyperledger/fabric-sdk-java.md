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
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    ignoring unnecessarily generated surefire report
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In our analysis, we observe that this target/surefire-report/ directory is generated but not later used during the CI build. Hence, we propose to disable generating this directory to save runtime.
The generation of this directory can be disabled by simply adding -DdisableXmlReport=true to the mvn command.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 17:25:13 +0000 UTC
    </div>
</div>

