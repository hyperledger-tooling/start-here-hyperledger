---
layout: default
title: fabric-admin-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-admin-sdk
---

# fabric-admin-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-admin-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/138" class=".btn">#138</a>
            </td>
            <td>
                <b>
                    Remove OSV-Scanner from vulnerability scan
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Running OSV-Scanner on the Node package-lock.json file could also detect vulnerabilities in dev dependencies. The intention of the vulnerability scan is to ensure that the production dependencies do not contain vulnerabilities, not the dev dependencies. This could be resolved by generating a Software Bill of Materials (SBOM) for the Node project, omitting dev dependencies, and running OSV-Scanner on the SBOM. Unfortunately, the use of non-semver tags (such as `latest`) in the dependency tree causes errors in npm ls when generating an SBOM.

Govulncheck and npm audit already do a good job of detecting vulnerabilities in Go and Node respectively so, for now at least, remove OSV-Scanner.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 16:54:04 +0000 UTC
    </div>
</div>

