---
layout: default
title: fabric-gateway-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway-java
---

# fabric-gateway-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway-java/pull/122" class=".btn">#122</a>
            </td>
            <td>
                <b>
                    Release v2.2.6
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
        Created At 2022-09-21 16:21:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway-java/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    Dependency updates and suppress vulnerability false positives (backport #120)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #120 done by [Mergify](https://mergify.com).


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
        Created At 2022-09-21 16:01:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway-java/pull/120" class=".btn">#120</a>
            </td>
            <td>
                <b>
                    Dependency updates and suppress vulnerability false positives
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
        Created At 2022-09-21 15:22:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway-java/pull/119" class=".btn">#119</a>
            </td>
            <td>
                <b>
                    Use correct CryptoSuite and User context for event replay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use the exact CryptoSuite and User context from the original HFClient when creating a new HFClient for event replay, instead of assuming that the CryptoSuite and User context are ones created using an X509IdentityProvider with the Gateway client identity.

Also updates dependency versions and fixed a compile warning in ContractException that could appear with Java 17.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-20 11:01:09 +0000 UTC
    </div>
</div>

