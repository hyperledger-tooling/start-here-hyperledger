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
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/205" class=".btn">#205</a>
            </td>
            <td>
                <b>
                    Fix bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                when I use fabric-sdk-go(my computer os is windows 10 ) to deploy chaincode,occur an error "Failed to generate platform-specific docker build: Error returned from build: 1 "can't load package: package github.com/testchaincode1: cannot find package "github.com/testchaincode1" in any of: ",but it can normal run in ubuntu,the sdk config almost same except tls and private key path, and they connect same fabric network.

I fix it by modify fabric-sdk-go,so I think It shoud be a bug
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 09:22:20 +0000 UTC
    </div>
</div>

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

