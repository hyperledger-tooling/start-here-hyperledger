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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/727" class=".btn">#727</a>
            </td>
            <td>
                <b>
                    add js cc for the private data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I was testing the private data concept, I noticed that the chaincode is only written with go and java then I decided to take this initiative and implement it with js, the cc was tested with the application I hope that would help js developers understand private data and use nodejs sdk easily.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 15:33:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/726" class=".btn">#726</a>
            </td>
            <td>
                <b>
                    Enable engine-strict checks for TypeScript Gateway samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use an .npmrc to enable engine-strict checks so that `npm install` will fail for projects when an incompatible Node version is used, rather than confusing errors about unsupported language features occuring at runtime.

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 13:30:08 +0000 UTC
    </div>
</div>

