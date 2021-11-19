---
layout: default
title: fabric-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-go
---

# fabric-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/203" class=".btn">#203</a>
            </td>
            <td>
                <b>
                    fix bug in validate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Json is stored alphabetically in couchdb, while golang "encoding/json" orders json by struct-field order. So, err could happened when user invoke/query peer with both couchdb-peer and leveldb-peer. The same problem could also happen when we use both javaCC and goCC.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 06:43:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/199" class=".btn">#199</a>
            </td>
            <td>
                <b>
                    fix typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wuqiaomin <wuqiaomin2@huawei.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 03:39:59 +0000 UTC
    </div>
</div>

