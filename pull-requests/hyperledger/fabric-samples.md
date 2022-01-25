---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/595" class=".btn">#595</a>
            </td>
            <td>
                <b>
                    ERC20 Java chaincode implementation exmaple.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: renjithkn@gmail.com <renjithkn@gmail.com>

This is an example of ERC20 token standard Java chaincode implementation.  The functionality is the same as the existing go and nodejs ERC20 chaincode.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 16:56:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/589" class=".btn">#589</a>
            </td>
            <td>
                <b>
                    Remove JCenter as a Gradle package repository
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                JCenter is deprecated, can no longer be published to, and is scheduled for removal. It is now causing build failures. Replace with Maven Central.

Also remove mavenLocal() as this is not recommended practice:
    
https://docs.gradle.org/current/userguide/declaring_repositories.html#sec:case-for-maven-local

Note that Jitpack still needs to be included as a package repository for Java chaincode since it has dependencies on an old version of com.github.everit-org.json-schema:org.everit.json.schema that is only published there.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 09:20:34 +0000 UTC
    </div>
</div>

