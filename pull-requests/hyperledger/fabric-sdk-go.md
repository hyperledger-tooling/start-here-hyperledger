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
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/221" class=".btn">#221</a>
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
        Created At 2022-02-07 03:21:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/219" class=".btn">#219</a>
            </td>
            <td>
                <b>
                    fix a bug on windows which will cause install chaincode failure
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
        Created At 2022-02-06 01:26:02 +0000 UTC
    </div>
</div>

