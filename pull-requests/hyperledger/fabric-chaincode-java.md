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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/314" class=".btn">#314</a>
            </td>
            <td>
                <b>
                    Update dependencies to address security vulnerabilities
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - CVE-2022-25647
- CVE-2023-2976
- CVE-2020-8908

Also:

- Update Gradle wrapper version to resolve Gradle bug in handling
  certain dependency JAR files.
- Update Gradle shadowJar plugin to v7.1.2 (except for bare-gradle contract,
  since builder uses Gradle v5 if no wrapper is provided).
- Add mergeServiceFiles() to test chaincode shadowJar Gradle tasks to
  resolve an issue with incorrect class versions being loaded from dependencies.
- Add ServicesResourceTransformer to test chaincode maven-shade-plugin
  Maven plugin configuration to resolve an issue with incorrect class
  versions being loaded from dependencies.
- Tidy-up integration test contract dependencies.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-20 14:51:20 +0000 UTC
    </div>
</div>

