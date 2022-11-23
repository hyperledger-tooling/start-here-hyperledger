---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/626" class=".btn">#626</a>
            </td>
            <td>
                <b>
                    Add Node 18 to Azure Pipelines publish build
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
        Created At 2022-11-23 09:42:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/625" class=".btn">#625</a>
            </td>
            <td>
                <b>
                    Add testing with Node 18 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @ampretia/x509 package does not work with Node 18 so changed to use jsrsasign to decode X.509 certificates in tests. This mostly works fine but seems to truncate non-standard extension values so some testing for custom attributes in CA enrollment are commented out for now.

Contributes to #621 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 18:57:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/624" class=".btn">#624</a>
            </td>
            <td>
                <b>
                    Downgrade nano dependency for backwards compatibility with Node 12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #623.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 13:11:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/622" class=".btn">#622</a>
            </td>
            <td>
                <b>
                    Add testing with Node 18
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @ampretia/x509 package does not work with Node 18 so changed to use jsrsasign to decode X.509 certificates in tests. This mostly works fine but seems to truncate non-standard extension values so some testing for custom attributes in CA enrollment are commented out for now.

Closes #621
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 10:44:15 +0000 UTC
    </div>
</div>

