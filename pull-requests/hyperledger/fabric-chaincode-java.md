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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/335" class=".btn">#335</a>
            </td>
            <td>
                <b>
                    Upgrade the version of JUnit vintage gradle used
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Again for CVE-2020-15250.


testImplementation 'org.junit.vintage:junit-vintage-engine:5.3.1' imports `junit:junit:4.12`... gotta move to `org.junit.vintage:junit-vintage-engine:5.10.2` to get to `junit:junit:4.13.2`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 18:55:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/333" class=".btn">#333</a>
            </td>
            <td>
                <b>
                    Move everything to latest fabric-protos (v0.3.3).
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The latest `fabic-protos` release is v0.3.3. I expect that all of our tests may fail using this version of the package, but I want to see where exactly the problem lies.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-06 19:39:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/332" class=".btn">#332</a>
            </td>
            <td>
                <b>
                    Use secure version of JUnit v4 for compilation.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://nvd.nist.gov/vuln/detail/CVE-2020-15250 indicates that `junit:junit:4.12` is insecure. But it has been patched and there's an easy fix to just move to v4.13.1.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-06 19:25:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/331" class=".btn">#331</a>
            </td>
            <td>
                <b>
                    Move Maven Contract Example to latest fabric-protos.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://nvd.nist.gov/vuln/detail/CVE-2022-3509, https://nvd.nist.gov/vuln/detail/CVE-2022-3171, and https://nvd.nist.gov/vuln/detail/CVE-2022-3510 all indicate issues with the `protobuf-java` dependency before a certain version.  The `fabric-protos` dependency at `0.2.1` is where most of the rest of this project sits, and it has no vulnerabilities.   Particularly, it uses `protobuf-java` v3.24.4. However, `fabric-protos` v0.1.3 imports an earlier version.  This **should** fix that problem.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-06 19:18:48 +0000 UTC
    </div>
</div>

