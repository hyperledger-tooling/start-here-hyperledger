---
layout: default
title: fabric-operator
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operator
---

# fabric-operator <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operator){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Use hyperledger-labs operator, not ibm-blockchain operator in sample network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After installing the operator about 50 times in test clusters, I was wondering why the image download counts from ghcr.io were still zero.  This would explain the issue... 

Sample network now pulls the LABS operator image, not the legacy rev (pre-labs).

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 01:20:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    Feature/bootstrap ca registration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR: 

- Optionally exposes the KIND / local docker insecure registry on alternate NICs, e.g. 0.0.0.0:9999.  (This encourages "remote" development patterns when building chaincode and gateway images locally on a host OS, then uploading into the k8s cluster without publishing to a public repo.)

- Runs a bootstrap `rcaadmin` client enrollment when setting up the CAs.  This allows a remote `fabric-ca-client` to register and enroll new user IDs directly at the org CA, without using the console GUI or ansible playbooks. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 18:34:00 +0000 UTC
    </div>
</div>

