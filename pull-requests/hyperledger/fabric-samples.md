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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/593" class=".btn">#593</a>
            </td>
            <td>
                <b>
                    ERC20 Java chaincode sample with unit test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an example of the Java chaincode implementation of the ERC20 token. It follows the same logic as the existing chain code in go and nodejs. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 05:11:24 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/586" class=".btn">#586</a>
            </td>
            <td>
                <b>
                    Fix: remove `shift` after `-verbose` 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are no argument after `-verbose`. So, it should not run `shift`.
If `-verbose` is not latest parameter, it will throw errro.
![image](https://user-images.githubusercontent.com/88102592/149860351-dac5abe4-c670-4e5b-b092-93f5d2c37b29.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 02:28:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/585" class=".btn">#585</a>
            </td>
            <td>
                <b>
                    Fix(commercial-paper): Fixed failed dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In branch release-1.4 , The path of "fabric-gateway-java" is no longer valid, fixed valid dependency

https://hyperledger.jfrog.io/ui/repos/tree/General/fabric-maven%2Forg%2Fhyperledger%2Ffabric-gateway-java%2F1.4.0-SNAPSHOT%2Ffabric-gateway-java-1.4.0-20200120.152501-1.pom

![image](https://user-images.githubusercontent.com/29918052/149764176-2d11300c-c767-4537-a1c6-9b685941da87.png)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-17 11:52:23 +0000 UTC
    </div>
</div>

