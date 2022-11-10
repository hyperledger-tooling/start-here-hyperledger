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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/852" class=".btn">#852</a>
            </td>
            <td>
                <b>
                    Moves the Full Stack Asset Transfer Development Guide to fabric-samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a step towards migrating the Hyperledgendary [Full Stack Asset Transfer](https://github.com/hyperledgendary/full-stack-asset-transfer-guide) Guide to fabric-samples.

This content was developed (and tested by fire!) as part of an interactive workshop at the HL Global Forum in 2022 in Dublin.  

The material covers: 
- Interactive and step-level debugging with CCaaS and microfab
- Interactive exercises and guidelines for building Gateway Client (Fabric > 2.4) based applications
- Interactive exercises and guides for deploying _cloud native_ Fabric networks and applications to local, hybrid, and public cloud.

The PR is generally a "pick up and move" from Hyperledgendary to the fabric-samples repo.   Some minor tweaks related to `$PWD` have been made to the READMEs and guides.

This PR includes some minor updates necessary to run the Kubernetes operator, Fabric network, and chaincode on an M1 / Mac running with the QEMU emulation.  (More work / testing in this area is necessary for the "local build" on the M1 for chaincode images running with the k8s builder.)

The last submission to the full-stack guide at the time of this import was at [commit fb554befdbbeff9e69159b54fce0b811603f29c7](https://github.com/hyperledgendary/full-stack-asset-transfer-guide/commit/fb554befdbbeff9e69159b54fce0b811603f29c7) on the remote repo ([PR #158](https://github.com/hyperledgendary/full-stack-asset-transfer-guide/pull/158).)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-09 21:52:49 +0000 UTC
    </div>
</div>

