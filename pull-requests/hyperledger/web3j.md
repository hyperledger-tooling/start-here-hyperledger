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
                PR <a href="https://github.com/hyperledger/web3j/pull/2068" class=".btn">#2068</a>
            </td>
            <td>
                <b>
                    Big fix for codegen when Array of struct and struct used together
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
 After fixing https://github.com/hyperledger/web3j/pull/2061, there is still an edge case where array of struct and struct are used together in the same contract e.g `Foo` and `Foo[2]`. Fix this by having `normalizeNamedType` to take care of static array

Also, structIdentifer is using hashCode which does not have uniqueness Property, it could subject to quite significant collision.

This should also fix https://github.com/hyperledger/web3j/issues/2056. Added test case for the example in the issue

### Where should the reviewer start?
All files

### Why is it needed?
Bug fix

## Checklist

- [x] I've read the contribution guidelines.
- [x] I've added tests (if applicable).
- [x] I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-14 19:19:39 +0000 UTC
    </div>
</div>

