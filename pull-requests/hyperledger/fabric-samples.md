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

