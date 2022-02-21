---
layout: default
title: fabric-gateway-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway-java
---

# fabric-gateway-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway-java/pull/101" class=".btn">#101</a>
            </td>
            <td>
                <b>
                    Fix Javadoc build for Java 17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Even if the path and compiler target point to a different Java version, the Java version associated with the Maven CLI can cause Javadodc build failures in systems with Java 17 installed. Set an upper bound (in addition to the lower bound) for the build profile that enables the `--no-module-directories` Javadoc option.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 09:57:50 +0000 UTC
    </div>
</div>

