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
                PR <a href="https://github.com/hyperledger/web3j/pull/2072" class=".btn">#2072</a>
            </td>
            <td>
                <b>
                    Document the minimum required Java version for the target project to use Web3j as a dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
This PR documents the minimum required Java version for the target project to use Web3j as a dependency

### Where should the reviewer start?
Relevant to the PR:

the current java version that is used for compilation:

https://github.com/hyperledger/web3j/blob/main/gradle/java/build.gradle
Somewhat relevant issue: https://github.com/hyperledger/web3j/issues/2069

### Why is it needed?

Users might encounter errors because Web3j doesn't compile with their project before they realize that the required version should be at least Java 17.

I think it will be beneficial for users to see the required Java version in the README, so they don't spend time digging into the Gradle parameters or troubleshooting issues while building their projects.


## Checklist

- [x] I've read the contribution guidelines.
- not applicable: I've added tests (if applicable).
- IMO a too smal change for a changelog entry. I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 20:30:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j/pull/2070" class=".btn">#2070</a>
            </td>
            <td>
                <b>
                    Bug fix for Int256 decode range [2^248, type(int256).max] and [ type(int256.min), -(2^248) )
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
Bug fix for decoding Int256 range [2^248, type(int256).max] and [ type(int256.min), -(2^248) )

### Where should the reviewer start?
All files

### Why is it needed?
The decoding of int256 number range  [2^248, type(int256).max] and [ type(int256.min), -(2^248) ) will throw exception,
type(int256.min) and type(int256).max is the particular case that we found


## Checklist

- [x] I've read the contribution guidelines.
- [x] I've added tests (if applicable).
- [x] I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-22 17:25:14 +0000 UTC
    </div>
</div>

