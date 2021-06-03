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
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/179" class=".btn">#179</a>
            </td>
            <td>
                <b>
                    bump go version check to allow go 1.16
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Version 1.16 has been released last February and is the current latest
stable release.

If there is a reason for not supporting the last stable release of go, feel free to close this PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 10:14:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/178" class=".btn">#178</a>
            </td>
            <td>
                <b>
                    fix findSource in javapackager/packager.go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 09:03:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/177" class=".btn">#177</a>
            </td>
            <td>
                <b>
                    Fixed a bug in proposal matcher when querying committed chaincodes. P…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes an error in the proposal matcher with an unexpected order of committed chaincodes returned from a peer. The matcher uses `proto.Equal` which fails to compare the values of slices that are in a different order.   
Two peers return the same list of the chaincodes in a slice instead of a map, that's why the order can't be guaranteed https://github.com/hyperledger/fabric/blob/main/core/chaincode/lifecycle/scc.go#L620.

Signed-off-by: Vladyslav Kopaihorodskyi <vlad.kopaygorodsky@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 15:50:55 +0000 UTC
    </div>
</div>

