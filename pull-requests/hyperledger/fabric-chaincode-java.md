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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/349" class=".btn">#349</a>
            </td>
            <td>
                <b>
                    Restore Java 8 compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Build with source and target bytecode compatibility for Java 8. This allows chaincode implementation code that requires Java 8 compatibility to compile against the fabric-chaincode-shim package.

Avoid use of mavenLocal() and (deprecated) jcenter() Gradle repositories.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-11 17:56:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/345" class=".btn">#345</a>
            </td>
            <td>
                <b>
                    Move to com.github.erosb:json-sKema:0.15.0 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `org.everit.erosb` is deprecated. See https://github.com/everit-org/json-schema?tab=readme-ov-file#deprecation-notice.  So there's a new schema, and also there are dependencies in the erosb fork that aren't going to be maintained, etc.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 14:58:46 +0000 UTC
    </div>
</div>

