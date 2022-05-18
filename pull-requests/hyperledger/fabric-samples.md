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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/746" class=".btn">#746</a>
            </td>
            <td>
                <b>
                    Update README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #740 

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 15:07:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/745" class=".btn">#745</a>
            </td>
            <td>
                <b>
                    fix to replace 443 with NGINX_HTTPS_PORT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                this fix replace hardcoded port 443 with NGINX_HTTPS_PORT which is useful in case ingress is installed on non conventional ports
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 13:53:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/744" class=".btn">#744</a>
            </td>
            <td>
                <b>
                    Fix typo in asset-transfer-basic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Tommy TIAN <xtianae@connect.ust.hk>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 13:09:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/742" class=".btn">#742</a>
            </td>
            <td>
                <b>
                    ERC token samples: Added final fixes to erc token samples and documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added a final fix to the go contract check for overflow
- added documentation for initialization of the contract in the READMEs
- include typos and idiomatic code fixes highlighted from comments of the last pr
Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 15:54:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/739" class=".btn">#739</a>
            </td>
            <td>
                <b>
                    Feature/fabric builder k8s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This (DRAFT) PR adds support for the [fabric-builder-k8s](https://github.com/hyperledgendary/fabric-builder-k8s) in the Kube Test Network.

fabric-builder-k8s is the missing "easy button" for working with Hyperledger Fabric Chaincode.  The builder is triggered by the existing "external builder" peer lifecycle events, managing the lifecycle of CC routines as pods under an RBAC-enabled service account.

With the k8s builder approach, chaincode ... "just works." 

### Background Context 

- [fabric-builder-k8s](https://github.com/hyperledgendary/fabric-builder-k8) - general overview
- Fabric Community Contributor Call [11 March ](https://wiki.hyperledger.org/download/attachments/62234113/20220511_contributors_meeting.mp4?api=v2) (> 0:11:00) k8s builder feature playback. 
- Fabric GitHub Discussion #3407 : [Default External Builder Approach for Kubernetes](https://github.com/hyperledger/fabric/discussions/3407)


### Installation / Activation
```
export TEST_NETWORK_CHAINCODE_BUILDER="k8s"

network kind 
network cluster init
network up 
network channel create
...
```

### Sample Chaincode Activation

- Set up the Kube test network as above 
- Install conga-nft-contract, starting at [running-peer-commands](https://github.com/hyperledgendary/fabric-builder-k8s/blob/main/docs/TEST_NETWORK_K8S.md#running-peer-commands)


### Open Items (this PR)

- E2E / functional test: 
  - build a KIND cluster, Fabric network, and channel 
  - compile chaincode sample (asset transfer) and docker image 
  - prepare a CC package referencing the CC docker image 
  - use `peer` CLI commands to instantiate, invoke, and query the CC 

- Improve the "release management" aspects of the builder source binaries: 
  - install via [pre-built binaries](https://github.com/hyperledgendary/fabric-builder-k8s/releases/tag/v0.1.0)?  (exec 'wget' in peer pod?)
  - install via [pre-built image](test-network-k8s/kube/org1/org1-install-k8s-builder.yaml)? (k8s job w/ copy to PV)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 16:42:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/738" class=".btn">#738</a>
            </td>
            <td>
                <b>
                    fix error message in deployCC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-13 10:06:48 +0000 UTC
    </div>
</div>

