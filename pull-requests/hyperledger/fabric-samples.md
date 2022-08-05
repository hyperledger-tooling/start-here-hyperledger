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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/808" class=".btn">#808</a>
            </td>
            <td>
                <b>
                    Clarifies podman instructions for test-network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also reverts to using install-fabric.sh which is preferred over bootstrap.sh.

Signed-off-by: Arnaud J Le Hors <lehors@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 16:43:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/806" class=".btn">#806</a>
            </td>
            <td>
                <b>
                    Add getCreator() to parsed transaction in off_chain_data sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Example of how the client identity that submitted a transaction can be obtained.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 09:43:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/805" class=".btn">#805</a>
            </td>
            <td>
                <b>
                    Update Node.js dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add options to stop permission issue with the npm cache (podman is quite strict here)
- Add in platform for tini

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 11:18:54 +0000 UTC
    </div>
</div>

