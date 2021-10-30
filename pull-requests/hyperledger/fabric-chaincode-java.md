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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/207" class=".btn">#207</a>
            </td>
            <td>
                <b>
                    cast type to java.nio.Buffer to flip()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When starting java chaincode as a service with shim 2.2.3 on JDK8, `epochBytes.flip()` throws `java.lang.NoSuchMethodError: java.nio.ByteBuffer.flip()`, which would make the response of the invoke request from peer miss, and peer would report timeout.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 18:22:33 +0000 UTC
    </div>
</div>

