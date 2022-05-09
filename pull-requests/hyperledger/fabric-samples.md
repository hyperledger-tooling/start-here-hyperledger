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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/733" class=".btn">#733</a>
            </td>
            <td>
                <b>
                    Update marbles_chaincode.go example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Running examples should work off-the-shelf. CouchDB now forces to use user_name & password for authentication. This patch fixes an existing example (marbles_chaincode) to work with the current requirements of CouchDB.

Signed-off-by: Obadah Hammoud <obadah.hammoud@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 17:06:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/731" class=".btn">#731</a>
            </td>
            <td>
                <b>
                    Updated ERC tokens samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added check for math oveflow where necessary - Closes #701
- added name, symbol and default token options to all go erc sample that were missing these options
- renamed `SetOptions()` to `Initialize()`
- made sure that you need to initialize contract and its options (call `Initialize()`) first before calling any contract functions
- made sure `Inizialized()` can be called only once

Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 16:42:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/729" class=".btn">#729</a>
            </td>
            <td>
                <b>
                    Run the Kube Test Network on Rancher / k3s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enables users of the Kube Test Network to set up a Fabric network based on k3s / [Rancher Desktop](https://rancherdesktop.io)

- Fixes #728 
- Upgrades Nginx ingress to 1.1.2 
- Aligns both KIND and Rancher runtimes to use the local-path provisioner

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 20:05:02 +0000 UTC
    </div>
</div>

