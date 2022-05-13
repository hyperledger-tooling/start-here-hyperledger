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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/736" class=".btn">#736</a>
            </td>
            <td>
                <b>
                    Off-chain data sample using Fabric Gateway client API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 14:45:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/735" class=".btn">#735</a>
            </td>
            <td>
                <b>
                    test-network-k8s: Add CC debugging procedures for Linux
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In chaincode debugging guidance, using the Docker host alias `host.docker.internal` is assumed.
But, the alias is not yet supported for Linux.
So, this patch adds its alternate procedure for Linux.

Signed-off-by: Tatsuya Sato <tatsuya.sato.so@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 01:54:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/734" class=".btn">#734</a>
            </td>
            <td>
                <b>
                    Fix creating channel when ${PWD} contains space. (backport #402)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">conflicts</span>
            </td>
            <td>
                This is an automatic backport of pull request #402 done by [Mergify](https://mergify.com).
Cherry-pick of 14dc7e13160ef1b7332bafb01f8ffa865116f9e7 has failed:
```
On branch mergify/bp/release-2.2/pr-402
Your branch is up to date with 'origin/release-2.2'.

You are currently cherry-picking commit 14dc7e1.
  (fix conflicts and run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes to be committed:
	modified:   asset-transfer-abac/README.md
	modified:   asset-transfer-basic/chaincode-external/README.md
	modified:   asset-transfer-sbe/README.md
	modified:   ci/templates/commercial-paper/azure-pipelines-go.yml
	modified:   ci/templates/commercial-paper/azure-pipelines-java.yml
	modified:   ci/templates/commercial-paper/azure-pipelines-javascript.yml
	modified:   commercial-paper/README.md
	modified:   commercial-paper/network-starter.sh
	modified:   commercial-paper/organization/digibank/digibank.sh
	modified:   commercial-paper/organization/magnetocorp/magnetocorp.sh
	modified:   interest_rate_swaps/network/network.sh
	modified:   test-network/addOrg3/fabric-ca/registerEnroll.sh
	modified:   test-network/network.sh
	modified:   test-network/organizations/fabric-ca/registerEnroll.sh
	modified:   test-network/scripts/configUpdate.sh
	modified:   test-network/scripts/deployCC.sh
	modified:   test-network/scripts/envVar.sh
	modified:   test-network/scripts/org3-scripts/joinChannel.sh
	modified:   test-network/scripts/org3-scripts/updateChannelConfig.sh
	modified:   test-network/scripts/setAnchorPeer.sh
	modified:   token-erc-20/README.md
	modified:   token-utxo/README.md

Unmerged paths:
  (use "git add <file>..." to mark resolution)
	both modified:   test-network/scripts/createChannel.sh

```


To fix up this pull request, you can check it out locally. See documentation: https://docs.github.com/en/github/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/checking-out-pull-requests-locally

---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 16:15:21 +0000 UTC
    </div>
</div>

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

