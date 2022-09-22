---
layout: default
title: iroha-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-java
---

# iroha-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    Introduced library plugin and opimized dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After lots of experiments I tested publishing to a maven repository instead of just building a JAR. With using `java-library` plugin we get a POM file near the jar contatining all needed transitive dependencies. So we need to adjust our CI to corporate registry (configure and execute task `publish` instead of copying the jars).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 13:12:17 +0000 UTC
    </div>
</div>

