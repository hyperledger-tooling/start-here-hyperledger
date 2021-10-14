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
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/517" class=".btn">#517</a>
            </td>
            <td>
                <b>
                    Fabric-Network 2 critical vulns with jsrsasign (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of 63fa2195d7c1981e3b28875a6e291608cee36d99 from main branch.

Resolves #500

* Bump jsrsasign from 8.0.24 to 10.4.1
* Primary changes made to support jsrsagin in Pkcs11EcdsaKey module
* replaced hexSig with sighex in csr object
* Changes made in CertificationRequest as per the new format
* Made changes in signCSR function as per jsrsasign package

Signed-off-by: Rajat Sharma <rajat.sharma@dltlabs.io>
Signed-off-by: Deepak Singh <deepak.singh2@dltlabs.io>
Co-authored-by: Rajat Sharma <rajat.sharma@dltlabs.io>
Co-authored-by: Deepak Singh <deepak.singh2@dltlabs.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 20:08:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/512" class=".btn">#512</a>
            </td>
            <td>
                <b>
                    [refactor] use override than type check switch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                An attempt to move if type=='query' check code block to inherit class
instead of expose too much subclass implementation detail in superclass

Signed-off-by: DavidLiu <david.yx.liu@oracle.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 04:01:33 +0000 UTC
    </div>
</div>

