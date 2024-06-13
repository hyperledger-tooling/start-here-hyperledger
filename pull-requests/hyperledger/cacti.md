---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3298" class=".btn">#3298</a>
            </td>
            <td>
                <b>
                    feat(fabric-connector): add getChainInfo, improve getBlock output
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add new method `getChainInfo` for quering chain information from qscc.
- Add `GetChainInfoEndpointV1` to allow calling `getChainInfo` remotely.
- Refactor `getBlock` so it can return same custom block formats as `WatchBlocks`. Default remains the same (full decode block). BREAKING CHANGE: It accepts `type` instead of `skipDecode` flag.
- Move common block formatting logic to `cacti-block-formatters.ts`.
- Add tests for new features. Move test common to quering `qscc` to single file to increase CI speed.

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 11:54:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3297" class=".btn">#3297</a>
            </td>
            <td>
                <b>
                    feat(satp-hermes): add skeleton for stage0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added the files for satp-hermes stage0. The logic is not final, just an adaptation of stage1 with a few changes in the message fields and names.

@RafaelAPB please have a look, to check if it is according to the intended architecture.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 08:59:29 +0000 UTC
    </div>
</div>

