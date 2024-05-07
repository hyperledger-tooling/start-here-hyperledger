---
layout: default
title: web3j
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/web3j
---

# web3j <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/web3j){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j/pull/2051" class=".btn">#2051</a>
            </td>
            <td>
                <b>
                    Upgrade gradle to v8.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
Fixes #2043 
Upgrades gradle to v8.0 and required upgrades to spotless and jacoco.

### Where should the reviewer start?
The gradle wrapper, followed by the `build.gradle` files.

### Why is it needed?
Upgrading a project to a Java version which requires a Gradle version >= 8.0 results in the deprecated method `setOutputDir` being removed which is used when generating java contract wrapper.

I tested this locally in a project using gradle v7.6 and v8.5.

## Checklist

- [x] I've read the contribution guidelines.
- [x] I've added tests (if applicable).
- [x] I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-07 15:28:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j/pull/2049" class=".btn">#2049</a>
            </td>
            <td>
                <b>
                    Bump snapshot version 4.11.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
Bump snapshot version 4.11.4

### Where should the reviewer start?
*required*

### Why is it needed?
*required*

## Checklist

- [x] I've read the contribution guidelines.
- [x] I've added tests (if applicable).
- [x] I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 14:40:56 +0000 UTC
    </div>
</div>

