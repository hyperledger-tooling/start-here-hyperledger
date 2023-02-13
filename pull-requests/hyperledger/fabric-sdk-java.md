---
layout: default
title: fabric-sdk-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-java
---

# fabric-sdk-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/262" class=".btn">#262</a>
            </td>
            <td>
                <b>
                    Allow client TLS certificate and key to be specified in connection profile (backport #261)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #261 done by [Mergify](https://mergify.com).


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
        Created At 2023-02-13 12:28:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    Allow client TLS certificate and key to be specified in connection profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I have done the changes as follows:

1. change property names from tlsClient* to client* in NetworkConfig.java; add unit test and associated fixture.
2. change from tlsClient* to client* in HFCAClient.java; add unit test and associated fixtures.
3. Refactor clientCert* and clientKey* to constant in Endpoint.java and apply the constants in Channel.java.

Closes #260
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-08 02:19:36 +0000 UTC
    </div>
</div>

