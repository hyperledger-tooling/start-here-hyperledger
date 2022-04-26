---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/563" class=".btn">#563</a>
            </td>
            <td>
                <b>
                    Fix license check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Always scan all files for license to avoid build failures after merging successfully building PRs. Change existing headers to consistently use SPDX form.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 11:19:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/562" class=".btn">#562</a>
            </td>
            <td>
                <b>
                    Ensure supported Node versions for all dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                klaw 4.x was named as a dependency of fabric-client and is also a transient dependency of recent versions of jsdoc. This version of klaw requires Node 14 and broke client applications using engine-strict.

Some other transient dev dependencies also caused issues with engine-strict enable so the versions of dependencies that reference them are locked down more tightly.

Add a .npmrc with engine-strict=true so Node version incompatibilities break the build.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 09:54:52 +0000 UTC
    </div>
</div>

