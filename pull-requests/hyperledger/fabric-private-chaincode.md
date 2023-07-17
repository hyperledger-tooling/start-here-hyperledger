---
layout: default
title: fabric-private-chaincode
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-private-chaincode
---

# fabric-private-chaincode <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-private-chaincode){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-private-chaincode/pull/713" class=".btn">#713</a>
            </td>
            <td>
                <b>
                    Resolves #693, upgrade ego to v1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                What this PR does / why we need it:
Upgrade ego to v1.3, current ego version is v1.0

Which issue(s) this PR fixes:

Fixes https://github.com/hyperledger/fabric-private-chaincode/issues/693

Special notes for your reviewer:
Successfully build docker-dev in local

can build local dev and test ego using the code below
```
cd $FPC_PATH/utils/docker
make build-dev
make run-dev
```

Here is the result:
```
root@docker-desktop:/project/src/github.com/hyperledger/fabric-private-chaincode# ego
EGo v1.3.0 (360a6a40836461465fdbd0742dfb0f980b68c638)
Manage and run EGo enclaves.
...
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 20:39:37 +0000 UTC
    </div>
</div>

