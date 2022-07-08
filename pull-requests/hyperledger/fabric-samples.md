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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/788" class=".btn">#788</a>
            </td>
            <td>
                <b>
                    Feature/ca v1.5.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR bumps the Kube test network to run with the latest patch build of Fabric (2.4) and Fabric CA (1.5) images. 

In addition, it re-organizes the setup script default environment variable declarations to align on column boundaries.  The old format was causing some "eye bleeding" when looking at the script.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 12:28:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/784" class=".btn">#784</a>
            </td>
            <td>
                <b>
                    Fix namespace in k8s configuration files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Issues:
1. When the name of NETWORK_NAME or NS in file "network" (i.e., the namespace in k8s) is changed from "test-network", the resources in the k8s cluster cannot be created successfully when the command "./network up" is executed.
Error message: error: the namespace from the provided object "test-network" does not match the namespace "xxxxxx". You must pass '--namespace=test-network' to perform this operation.
2. org2-cc.yaml is not completed.

Fix:
1. Replace "test-network" in yaml files in folder "kube" with "${NS}".
2. Complete "org2-cc-template.yaml" by referring to "org1-cc-template.yaml".
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 09:53:11 +0000 UTC
    </div>
</div>

