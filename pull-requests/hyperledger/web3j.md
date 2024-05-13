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
                PR <a href="https://github.com/hyperledger/web3j/pull/2054" class=".btn">#2054</a>
            </td>
            <td>
                <b>
                    Fixed DefaultFunctionEncoder calculating offset for nested StaticArray
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
This PR fixed DefaultFunctionEncoder calculates offset for nested StaticStruct.
That's the problem that's bothering me right now.
See [issue-2052](https://github.com/hyperledger/web3j/issues/2052) for details

### Where should the reviewer start?
Look at the getLength function of DefaultFunctionEncoder.java changes.

### Why is it needed?
In slightly complex nested structures, calculate offset via getLength is incorrect. This is a bug that needs to be fixed.

## Checklist

- [ ] I've read the contribution guidelines.
- [ ] I've added tests (if applicable).
- [ ] I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 13:36:41 +0000 UTC
    </div>
</div>

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

