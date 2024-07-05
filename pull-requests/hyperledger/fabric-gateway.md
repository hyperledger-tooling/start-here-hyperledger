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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/731" class=".btn">#731</a>
            </td>
            <td>
                <b>
                    Add pkcs11 Go build tag to CodeQL autobuild
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allows CodeQL to scan Go files excluded by this build contraint.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-05 09:30:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/729" class=".btn">#729</a>
            </td>
            <td>
                <b>
                    Use current Go version for OSV-Scanner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                OSV-Scanner uses the Go version specified by the `go` line in the `go.mod` file. The patch level specified is deliberately a lower version than the latest to allow consumers to select their own Go patch level, provided that the major / minor version are at the required level. This behaviour results in OSV-Scanner detecting standard library vulnerabilities from the back-level Go patch level.

This change forces OSV-Scanner to use the exact version of the Go binary used to run the scan.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 18:34:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/728" class=".btn">#728</a>
            </td>
            <td>
                <b>
                    Update PMD version used for Java static analysis
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
        Created At 2024-07-01 14:57:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/727" class=".btn">#727</a>
            </td>
            <td>
                <b>
                    Add support for Node 22
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
        Created At 2024-06-29 17:05:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/726" class=".btn">#726</a>
            </td>
            <td>
                <b>
                    Use Java dependency-check GitHub Action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Maven dependency-check plugin is tricky to run due to:

- Need for NVD API token.
- Need to cache vulnerability database to avoid downloading the whole database on every invocation.
- Unreliability of the NVD API endpoint.

The action uses a Docker container that includes an up-to-date copy of the vulnerability database so avoids the need to use the NVD API.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-29 16:04:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/725" class=".btn">#725</a>
            </td>
            <td>
                <b>
                    Use full go version in go.mod
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                From Go 1.21, in the absence of a toolchain line in the go.mod file, the go line is used as the minimum toolchain version. Toolchain versions must be a full Go version, including patch level.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-29 12:07:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/724" class=".btn">#724</a>
            </td>
            <td>
                <b>
                    Remove CycloneDX Java SBOM generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was used to generate an SBOM containing transitive dependencies for OSV-Scanner. OSV-Scanner v1.8.1 and later can natively scan transitive dependencies in Maven pom.xml files so the CycloneDX SBOM generation step is no longer required.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-29 08:04:12 +0000 UTC
    </div>
</div>

