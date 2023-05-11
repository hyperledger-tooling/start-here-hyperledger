---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1302" class=".btn">#1302</a>
            </td>
            <td>
                <b>
                    Update Fabric chaincode Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Building with this Dockerfile currently breaks because the batchpin folder isn't being copied


```#10 2.414 go: downloading golang.org/x/text v0.3.2
#10 5.161 chaincode/contract.go:8:2: no required module provides package github.com/hyperledger/firefly/chaincode-go/batchpin; to add it:
#10 5.161       go get github.com/hyperledger/firefly/chaincode-go/batchpin
------
executor failed running [/bin/sh -c ls -la ./     && GO111MODULE=on GOOS=linux CGO_ENABLED=0 go build -o firefly.bin firefly.go]: exit code: 1```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 19:13:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1300" class=".btn">#1300</a>
            </td>
            <td>
                <b>
                    fix: missing test coverage
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
        Created At 2023-05-05 12:40:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1299" class=".btn">#1299</a>
            </td>
            <td>
                <b>
                    Fix unique indexes for transfers/approvals to be per-namespace
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
        Created At 2023-05-04 16:54:10 +0000 UTC
    </div>
</div>

