---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/812" class=".btn">#812</a>
            </td>
            <td>
                <b>
                    Refactor Go files, remove/replace deprecated functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Replace deprecated ioutil functions: ioutil is deprecated as of Go 1.16. The same functionality is now provided by package io or package os, and those implementations should be preferred in new code.
2. Fix variable names that collide with imported package name: "gateway" and "status" in [asset-transfer-basic/application-gateway-go/assetTransfer.go](https://github.com/hyperledger/fabric-samples/compare/main...tommytim0515:fabric-samples:fix_deprecated_ioutil?expand=1#diff-d4ed6defeea358911610bc1ea479c70f9f2a4707fc5c33cfad2a98f113b6692a) collide with names of the packages imported.
4. Fix typos.

Signed-off-by: Tommy TIAN <xtianae@connect.ust.hk>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-06 13:40:15 +0000 UTC
    </div>
</div>

