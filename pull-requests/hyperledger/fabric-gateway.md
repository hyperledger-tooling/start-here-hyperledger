---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/155" class=".btn">#155</a>
            </td>
            <td>
                <b>
                    Publish nightly builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit reverts changes to debug Java publish problems

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-02 10:16:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/154" class=".btn">#154</a>
            </td>
            <td>
                <b>
                    Java event example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 19:38:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/153" class=".btn">#153</a>
            </td>
            <td>
                <b>
                    Update repository ID in Java pom.xml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                maven-artifactory didn’t fix the 401 problem so reverting to maven-artifactory which
was the ID for the last successful publish.

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 17:05:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Sample should pull node SDK from NPM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 15:38:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/151" class=".btn">#151</a>
            </td>
            <td>
                <b>
                    Update repository ID in Java pom.xml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Java publish is broken due to a 401 error

Attempting to fix by changing the id to match the maven service connection ID…

“You should set the repositories in your project's pom.xml to have the same <id> as the name specified in the task for Maven to be able to correctly authenticate the task.”

https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/package/maven-authenticate?view=azure-devops
Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-29 15:16:33 +0000 UTC
    </div>
</div>

