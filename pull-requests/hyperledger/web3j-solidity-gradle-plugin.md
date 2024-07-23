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
                PR <a href="https://github.com/hyperledger/web3j-solidity-gradle-plugin/pull/75" class=".btn">#75</a>
            </td>
            <td>
                <b>
                    Make the 'prettyJson' option work
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?

`options.add(options.add("--$OutputComponent.ASM_JSON"))` contained a duplicated `options.add`, which added `true` to the command line (the return value of `options.add()`). The command fails with: _unrecognized "true"_.

This PR proposes to fix this issue by not implicitly adding the additional `ASM_JSON` output. As  `prettyJson = true` also makes sense in combination with other outputs such as `ABI`.

### Where should the reviewer start?

n/a

### Why is it needed?

`prettyJson = true` is currently not working. It always leads to a broken compiler call.


## Checklist

- [x] I've read the contribution guidelines.
- [ ] I've added tests (if applicable).
- [x] I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-23 11:56:38 +0000 UTC
    </div>
</div>

