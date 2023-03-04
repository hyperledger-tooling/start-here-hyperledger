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
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/566" class=".btn">#566</a>
            </td>
            <td>
                <b>
                    Use effective POM for osv-scanner to include transitive dependencies
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
        Created At 2023-02-28 17:49:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/565" class=".btn">#565</a>
            </td>
            <td>
                <b>
                    Use @noble/curves for Node signing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This package is newer than elliptic, has fewer dependencies, is better typed, and appears to be faster.

Closes #524
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 14:40:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/564" class=".btn">#564</a>
            </td>
            <td>
                <b>
                    Use explicit lockfile argument to osv-scanner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A behavioural change in osv-scanner meant that files included in a .gitignore file were ignored. This prevented the package-lock.json from being scanned. Explicitly specifying the file to be scanned using the --lockfile paramter avoids this issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-26 21:12:33 +0000 UTC
    </div>
</div>

