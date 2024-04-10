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
                PR <a href="https://github.com/hyperledger/web3j-gradle-plugin/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    Use Gradle 8 compatible API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
### What does this PR do?
In Web3JGradle plugin replace an API that was removed in Gradle 8 with a
Gradle 8 API and an appropriate fallback.

### Where should the reviewer start?
PR is only a few lines, should be self-evident.

### Why is it needed?
The old getOutputDir API has been removed in Gradle 8.  This prevents 
the plugin from being used in Gradle 8. The chagnes use a compatable API
that also falls back to the original code if used in a very old Gradle 7
build.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-08 02:50:54 +0000 UTC
    </div>
</div>

