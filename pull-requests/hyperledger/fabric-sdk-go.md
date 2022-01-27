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
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/216" class=".btn">#216</a>
            </td>
            <td>
                <b>
                    pkg/fab/ccpackager/javapackager: fix bug in findSoucrce
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Relpath of "META-INF/xxx" could be longer than folderpath, then filepath will be incomplete.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 07:32:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/215" class=".btn">#215</a>
            </td>
            <td>
                <b>
                    pkg/client/channel/invoke: fix bug in validate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When using couchdb, Json is stored alphabetically, while golang "encoding/json" orders json by struct-field order. There could be an error when user invoke/query peer with both couchdb-peer and leveldb-peer. The same problem could also happen when we use both javaCC and goCC.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 10:03:56 +0000 UTC
    </div>
</div>

