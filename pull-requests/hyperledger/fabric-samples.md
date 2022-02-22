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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/652" class=".btn">#652</a>
            </td>
            <td>
                <b>
                    refactor folder structure to match other token samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                hey @mbwhite whenever you had a moment, this is just a refactor of folder structure request by the community so that it matches the same structure as other token samples. Thanks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-19 15:55:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/651" class=".btn">#651</a>
            </td>
            <td>
                <b>
                    impl for couchdb supports in test0network8s as hardcode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                a impl for #633

Signed-off-by: Sam Yuan <yy19902439@126.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-19 12:10:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/650" class=".btn">#650</a>
            </td>
            <td>
                <b>
                    Add external chaincode service for Nano Test Network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This addresses Issue #504. This extends the test-network-nano-bash
sample to offer an option to run a fabric network without using any
containers at all. The chaincode is running as an external service
directly on the host machine.

Signed-off-by: Arnaud J Le Hors <lehors@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 15:35:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/649" class=".btn">#649</a>
            </td>
            <td>
                <b>
                    fix docker compose version 2 -> 2.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Earlier compose version was giving a property error when running the [fabric-samples/test-network/network.sh](https://github.com/hyperledger/fabric-samples/blob/main/test-network/network.sh) script.
![compose_error](https://user-images.githubusercontent.com/16841301/154474662-ceb92110-ba54-4887-935d-bc0db32da006.png)

Docker Compose Documentation says that the property [networks:name](https://docs.docker.com/compose/compose-file/compose-file-v2/#name-1) was added in [v2.1](https://docs.docker.com/compose/compose-file/compose-versioning/#version-21) file format.
Signed-off-by: kaushikkumarbora <kaushikkumarbora@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 11:47:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/647" class=".btn">#647</a>
            </td>
            <td>
                <b>
                    Improve REST sample README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add that one needs to have the ledger initialized for the sample to
work.

Signed-off-by: Arnaud J Le Hors <lehors@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 10:49:53 +0000 UTC
    </div>
</div>

