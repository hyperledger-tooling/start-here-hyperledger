---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4068" class=".btn">#4068</a>
            </td>
            <td>
                <b>
                    Home Button and Text of Side Navigation Menu (backport #4038)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4038 done by [Mergify](https://mergify.com).


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
        Created At 2023-02-27 13:55:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4067" class=".btn">#4067</a>
            </td>
            <td>
                <b>
                    GetIdemixMspConfig should require signerBytes not nil
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                GetIdemixMspConfig should require signerBytes not nil so that msp.Setup() do not panic

#### Type of change
- Improvement

#### Description

The GetIdemixMspConfig function ignores errors that the SignerConfig file is empty or does not exist. This causes a panic when the MSP is initialized later.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-26 13:05:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4064" class=".btn">#4064</a>
            </td>
            <td>
                <b>
                    BFT review comments: channelparticipation.Join
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I92a347a6105fbe99e934f8d4686378e58eb984ce


#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
Addressing review comments on the modification of channelparticipation.Join in the BFT commit.
This reverses the changes made to channelparticipation.Join in the BFT commit and fixes the respective tests accordingly.

Add retry to forwarding of the config-tx that causes a leader to abdicate, reducing the changes of integration test flakes.

#### Related issues
Raft IT flake #4066 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-23 14:17:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4058" class=".btn">#4058</a>
            </td>
            <td>
                <b>
                    Address comments on BFT PR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-21 14:45:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4057" class=".btn">#4057</a>
            </td>
            <td>
                <b>
                    Async connections to endpoints (backport #4050)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4050 done by [Mergify](https://mergify.com).


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
        Created At 2023-02-21 08:34:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4056" class=".btn">#4056</a>
            </td>
            <td>
                <b>
                    Async connections to endpoints (backport #4050)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4050 done by [Mergify](https://mergify.com).


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
        Created At 2023-02-21 08:33:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4055" class=".btn">#4055</a>
            </td>
            <td>
                <b>
                    Revert github.com/prometheus/client_golang to v1.11.1 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The bump to v1.14.0 causes Fabric compilation issues on ubuntu docker images.
See issue #4052 for details about the problematic build tag.
For now, it is acceptable to revert to v1.11.1 where there is no such build tag.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-20 21:41:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4054" class=".btn">#4054</a>
            </td>
            <td>
                <b>
                    Revert github.com/prometheus/client_golang to v1.11.1 (main)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The bump to v1.14.0 causes Fabric compilation issues on ubuntu docker images.
See issue hyperledger#4052 for details about the problematic build tag.
For now, it is acceptable to revert to v1.11.1 where there is no such build tag.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-20 21:37:50 +0000 UTC
    </div>
</div>

