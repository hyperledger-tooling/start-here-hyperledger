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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/325" class=".btn">#325</a>
            </td>
            <td>
                <b>
                    Fix image names in Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 16:26:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/324" class=".btn">#324</a>
            </td>
            <td>
                <b>
                    Fix test workflow link in release workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 15:37:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/323" class=".btn">#323</a>
            </td>
            <td>
                <b>
                    Prepare for v2.5.1 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update version numbers.
- Update GitHub Actions versions.
- Update base Java 11 Docker image patch level.
- Upgrade Gradle and Maven patch levels in Docker image.
- Update dependencies.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-06 21:46:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/322" class=".btn">#322</a>
            </td>
            <td>
                <b>
                    Address CVE-2023-6481 by moving to logback v1.3.14.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As per https://nvd.nist.gov/vuln/detail/CVE-2023-6481
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-06 14:23:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/321" class=".btn">#321</a>
            </td>
            <td>
                <b>
                    Use OSV-Scanner instead of dependency-check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The existing dependency-check version is no longer supported and might fail after the NVD data feeds it uses are deprecated on 2023-12-15. The updated version requires an API key to interact with the newer NVD APIs. For details see:

- https://github.com/jeremylong/DependencyCheck#900-upgrade-notice

It also requires periodic triage and suppression of false positive detections. OSV-Scanner appears less prone to false positives and does not require an API key to be maintained.

Implement a scheduled vulnerability scan (using OSV-Scanner) so that vulnerabilities are more visible than the current (dependency-check) implementation, which runs in PR builds but does not fail builds or make the results very visible.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 17:25:35 +0000 UTC
    </div>
</div>

