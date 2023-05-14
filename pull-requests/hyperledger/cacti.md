---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2424" class=".btn">#2424</a>
            </td>
            <td>
                <b>
                    fix(webpack): fix broken bundling - cannot find webpack.config.js
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `examples/cactus-workshop-examples-2022-11-14` package was causing `yarn build:dev` to fail. This PR fixes the incorrect webpack config path in the example's `package.json` file and adds a missing `/src/main/typescript/index.web.ts` file.
Fixes https://github.com/hyperledger/cacti/issues/2357
Signed-off-by: deepto98 [ddepp98@outlook.com](mailto:ddepp98@outlook.com)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-14 15:43:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2422" class=".btn">#2422</a>
            </td>
            <td>
                <b>
                    chore(release): publish v2.0.0-alpha-prerelease
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Testing release with `alpha-prerelease`.

Have to change `gomodule` names due to golang mandatory requirement that any version with v2 or above, must have major version suffixed to the `gomodule` name. Also had to modify `go-gen-checksum` script according to this convention.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-11 04:07:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2420" class=".btn">#2420</a>
            </td>
            <td>
                <b>
                    chore(ci): update actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                many actions were using old versions.

update rtd so docs build.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 14:35:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2418" class=".btn">#2418</a>
            </td>
            <td>
                <b>
                    feat: add private htlcs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                adds private htlcs to the htlc package (with tests)
updates non-rivate htlc contract
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 23:59:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2417" class=".btn">#2417</a>
            </td>
            <td>
                <b>
                    feat(connector-tcs-huawei):  Initial commit of feature tcs-huawei connector.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                tcs-huawei and the blockchains connected to tcs-huawei can be integrated to cactus by this connector.

Signed-off-by: Wang Yinglun wangyinglun3@huawei.com 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 06:19:16 +0000 UTC
    </div>
</div>

