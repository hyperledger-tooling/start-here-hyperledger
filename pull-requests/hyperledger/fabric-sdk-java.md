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
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    Run vulnerability scan only in the nightly build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update scan version
- Add suppression of vulnerability false positive
- Fix Javadoc build for later Java versions
- Run integration tests with Java 8, 11 and 17

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 18:21:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    upgrade opentelemetry version to 1.12.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I have projects using [fabric-sdk-java](https://github.com/hyperledger/fabric-sdk-java) that also use opentelemetry at `1.12.0`, which clashes with the transitive dependency from here. Would appreciate if we can upgrade it to the latest version of 1.12.0. 

@bestbeforetoday could someone please help me figure out what went wrong with the build here?

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 12:56:58 +0000 UTC
    </div>
</div>

