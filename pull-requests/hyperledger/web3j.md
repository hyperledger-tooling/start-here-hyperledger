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

