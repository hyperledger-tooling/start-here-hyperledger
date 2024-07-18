---
layout: default
title: web3j-gradle-plugin
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/web3j-gradle-plugin
---

# web3j-gradle-plugin <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/web3j-gradle-plugin){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j-gradle-plugin/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    feat: Add generate both flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
This PR adds a **generateBoth** flag to the plugin. 
GenerateContractWrapper.java forwards parameters to SolidityFunctionWrapperGenerator in codegen which has an optional parameter **generateBoth**. This parameter is currently not exposed in the plugin so this pr aims to expose it.

### Where should the reviewer start?
`GenerateContractWrapper.java`

### Why is it needed?
We want to integrate the web3j-plugin in hedera-mirror-node integration tests and this flag will really help.

## Checklist

- [x] I've read the contribution guidelines.
- [x] I've added tests (if applicable).
- [x] I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 17:40:39 +0000 UTC
    </div>
</div>

