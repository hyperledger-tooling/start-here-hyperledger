---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.4.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.4.19
                </span>
            </td>
            <td>
                This is a maintenance release that updates the [jsrsasign](https://www.npmjs.com/package/jsrsasign) dependency version to address a security vulnerability in RSA signature validation:

- [CVE-2021-30246](https://github.com/advisories/GHSA-27fj-mc8w-j9wg)

Note that the Node SDK does not perform RSA signature validation and so should not have been impacted by this vulnerability.
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/fabric-sdk-node/releases/tag/v1.4.19" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-01-19 07:55:03 +0000 UTC
    </span>
</div>

