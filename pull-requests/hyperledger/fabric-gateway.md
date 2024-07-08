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

