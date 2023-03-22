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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1011" class=".btn">#1011</a>
            </td>
            <td>
                <b>
                    Fixed fabric-samples/asset-transfer-basic/application-gateway-typescr…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed fabric-samples/asset-transfer-basic/application-gateway-typescript grpc client type check
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 19:16:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1010" class=".btn">#1010</a>
            </td>
            <td>
                <b>
                    Add in examples and notes on using PurgePrivateData
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update the configtx.yaml to enable the 2.5 capabillity
- Added purge into the chaincode
- Added purge into the application client code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-17 14:02:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1009" class=".btn">#1009</a>
            </td>
            <td>
                <b>
                    Remove csr.hosts from msp enrollments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Flag --csr.hosts is only relevant for tls enrollments, it adds the SAN to the TLS cert.
For msp enrollments, the cert is only used for identity, therefore there is no need for SAN and no need to pass --csr.hosts. 
Having --csr.hosts for msp enrollments is misleading, this commit removes it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-15 19:10:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1008" class=".btn">#1008</a>
            </td>
            <td>
                <b>
                    Bump couchdb to 3.2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump couchdb to 3.2.2.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-15 15:42:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1007" class=".btn">#1007</a>
            </td>
            <td>
                <b>
                    Add debug logging to CI scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add debug logging to CI scripts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-15 15:05:23 +0000 UTC
    </div>
</div>

