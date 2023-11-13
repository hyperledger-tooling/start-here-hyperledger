---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v2.2.20
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.2.20
                </span>
            </td>
            <td>
                ## What's Changed
* Update dependencies to address CVE-2023-45857 by @bestbeforetoday in https://github.com/hyperledger/fabric-sdk-node/pull/689

## Supported Node versions

The updated dependency to address CVE-2023-45857 is used only by the CouchDB wallet implementation, and requires Node 14 or later. Therefore Node 10 and 12 are no longer supported by the **fabric-network** package. If you need to continue running on one of these unsupported Node versions, you should continue to use **fabric-network@2.2.19**.

**Full Changelog**: https://github.com/hyperledger/fabric-sdk-node/compare/v2.2.19...v2.2.20
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric-sdk-node/releases/tag/v2.2.20" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-11-13 12:29:15 +0000 UTC
    </span>
</div>

