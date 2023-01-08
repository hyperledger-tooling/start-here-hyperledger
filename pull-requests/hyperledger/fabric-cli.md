---
layout: default
title: fabric-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-cli
---

# fabric-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-cli/pull/43" class=".btn">#43</a>
            </td>
            <td>
                <b>
                    Add missing properties to collections generation from bytes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In function GetCollectionsConfigFromBytes, it was not possible to get a config file with properties MemberOnlyRead, MemberOnlyWrite and BlockToLive even though protos types had the properties.

With this PR, the missing properties are now filled for the proto generation.

Signed-off-by: Samuel Venzi <samuel.venzi@me.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-08 11:47:35 +0000 UTC
    </div>
</div>

