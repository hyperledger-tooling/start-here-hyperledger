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
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/568" class=".btn">#568</a>
            </td>
            <td>
                <b>
                    Bug fix #548
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
        Created At 2022-04-27 12:22:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/566" class=".btn">#566</a>
            </td>
            <td>
                <b>
                    Update nconf dependency to address CVE-2022-21803
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #561
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 10:23:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/565" class=".btn">#565</a>
            </td>
            <td>
                <b>
                    Define endorseTimeout value in fabric-sdk-node v1.4(Issue #552)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In fabric-sdk-node v1.4, as well as in v2.2, define "endorseTimeout" value and use it instead of commitTimeout.

Co-Authored-by: Shinsuke Hasegawa <shinsuke.hasegawa.fc@hitachi.com>
Signed-off-by: takayuki-nagai <takayuki.nagai.nu@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 15:16:43 +0000 UTC
    </div>
</div>

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

