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
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/292" class=".btn">#292</a>
            </td>
            <td>
                <b>
                    Update dependencies to address CVE-2023-3635
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added explicit dependency on okio-bom to force the transitive okio dependency to a non-vulnerable version. This can be removed once okhttp 4.12 is eventually published and opentelemetry publishes a version that depends on it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 00:12:46 +0000 UTC
    </div>
</div>

