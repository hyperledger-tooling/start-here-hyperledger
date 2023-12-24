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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/666" class=".btn">#666</a>
            </td>
            <td>
                <b>
                    Go vulnerability scan configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove deprecated experimental-call-analysis flag. Call analysis is no longer experimental and is enabled by default for Go.
- Specify pkcs11 build tag in govulncheck scan to include HSM code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-24 01:57:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/665" class=".btn">#665</a>
            </td>
            <td>
                <b>
                    Fix Cucumber typings in Node scenario tests
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
        Created At 2023-12-22 20:43:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/663" class=".btn">#663</a>
            </td>
            <td>
                <b>
                    Define NVD_API_KEY in vulnerability scan
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use the NVD_API_KEY secret to access vulnerability definitions from the NVD database.

Temporarily disable dependency-check scan since the current version appears to run unreliably in GitHub Actions, although it works locally.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-20 22:28:20 +0000 UTC
    </div>
</div>

