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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/812" class=".btn">#812</a>
            </td>
            <td>
                <b>
                    Refactor Go files, remove/replace deprecated functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Replace deprecated ioutil functions: ioutil is deprecated as of Go 1.16. The same functionality is now provided by package io or package os, and those implementations should be preferred in new code.
2. Fix variable names that collide with imported package name: "gateway" and "status" in [asset-transfer-basic/application-gateway-go/assetTransfer.go](https://github.com/hyperledger/fabric-samples/compare/main...tommytim0515:fabric-samples:fix_deprecated_ioutil?expand=1#diff-d4ed6defeea358911610bc1ea479c70f9f2a4707fc5c33cfad2a98f113b6692a) collide with names of the packages imported.
4. Fix typos.

Signed-off-by: Tommy TIAN <xtianae@connect.ust.hk>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-06 13:40:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/811" class=".btn">#811</a>
            </td>
            <td>
                <b>
                    Update k8s CC builder to v7.2; Use *.localho.st loopback domain; Optionally bind docker reg to 0.0.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR: 

- The default k8s chaincode builder is upgraded from version 0.6.0 to 0.7.2 

- The `TEST_NETWORK_LOCAL_REGISTRY_INTERFACE` setting can be used to optionally bind the local docker insecure registry to an arbitrary NIC.  By default the registry is bound to the loopback interface 127.0.0.1 

- Switches from `*.vcap.me` to `*.localho.st` for the local host DNS wildcard domain.  (vcap.me is a remnant of an antiquated VMWare product.  Both domain names will match a wildcard to 127.0.0.1 in public DNS.) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-06 11:45:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/809" class=".btn">#809</a>
            </td>
            <td>
                <b>
                    Run RCAADMIN registration on the host OS, not in k8s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR changes the initial CA bootstrap enrollment to run on the _host_ OS, leaving an MSP folder structure on the local storage.  This greatly simplifies the process of registering additional node, client, and admin users with a local `fabric-ca-client` binary. 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 22:44:25 +0000 UTC
    </div>
</div>

