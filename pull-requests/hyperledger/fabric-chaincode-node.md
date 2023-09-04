---
layout: default
title: fabric-chaincode-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-node
---

# fabric-chaincode-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/406" class=".btn">#406</a>
            </td>
            <td>
                <b>
                    Avoid build failure due to warning running docker build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rush interpreted output to stderr from the docker build command as a build warning. This failed the build pipeline.

Also:

- Update version of Rush and pnpm.
- Remove use of toolchain package since it has been unpublished from the npm registry.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-03 22:07:23 +0000 UTC
    </div>
</div>

