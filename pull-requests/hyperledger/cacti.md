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
                PR <a href="https://github.com/hyperledger/cacti/pull/3036" class=".btn">#3036</a>
            </td>
            <td>
                <b>
                    docs(build): change NodeJS version in BUILD.md to v18.18.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fix node version in BUILD.md what caused type error in corepack
and prevented yarn from installing packages correctly.
Error message when using node 16: Type Error: URL.canParse is not a function

Signed-off-by: Tomasz Awramski <tomasz.awramski@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 14:23:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3035" class=".btn">#3035</a>
            </td>
            <td>
                <b>
                    test(cbdc-example): removed dependency on chai and update tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Chai was removed as dependency of the cbdc-backend package
* A test scenario was removed in the 'bridge-back' feature due to having duplicated logic with another one in the same file
* Some tests were failing due to timeouts, so we added an explicit and generous timeout limit for each step

closes #3034
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-28 17:07:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3033" class=".btn">#3033</a>
            </td>
            <td>
                <b>
                    chore: make spellcheck script less noisy with --no-progress flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A quality of life improvement for contributors.

Prior to this the cspell tool that we invoke for spellchecking had listed every single file as a separate log line on standard output during it's execution and the files that had issues were marked in that list, but since we have more than a thousand files, it was a lot of scrolling and scanning to find the files that had spelling mistakes in them during development time.

With the `--no-progress` flag now passed in to cspell it will only print the files that were found to have spelling mistakes in them which makes contributor productivity a little better.

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
        Created At 2024-02-28 01:54:10 +0000 UTC
    </div>
</div>

