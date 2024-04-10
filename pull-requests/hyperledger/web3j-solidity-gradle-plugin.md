---
layout: default
title: web3j-solidity-gradle-plugin
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/web3j-solidity-gradle-plugin
---

# web3j-solidity-gradle-plugin <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/web3j-solidity-gradle-plugin){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j-solidity-gradle-plugin/pull/67" class=".btn">#67</a>
            </td>
            <td>
                <b>
                    Gradle 8 compatability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
### What does this PR do?
This applies the essential fixes needed to upgrade to Gradle 8.6 but
continues to use Gradle 7.6 in the plugin build system. This provides
for Gradle 8.x compatability.

### Where should the reviewer start?
These are two small changes focused on the outputDir proeprty and one
fix that will be needed to test with Gradle 8

### Why is it needed?
Without these changes the plugin cannot be used in Gradle 8.x, which
is required for Java 21 support.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-08 02:57:06 +0000 UTC
    </div>
</div>

