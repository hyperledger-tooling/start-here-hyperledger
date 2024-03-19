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
                PR <a href="https://github.com/hyperledger/cacti/pull/3083" class=".btn">#3083</a>
            </td>
            <td>
                <b>
                    refactor(gui): gui structure change to make adding more ledgers easier
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - change folder structure
- each ledger-plugin now has separate folder and configuration
- added status page for available plugins
    
 Signed-off-by: Tomasz Awramski <tomasz.awramski@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-13 17:08:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3082" class=".btn">#3082</a>
            </td>
            <td>
                <b>
                    test(connector-fabric): move integration tests to use Fabric v2.5.6 AIO
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. This fixes many flakes that we were suffering from before with the
older versions of the AIO image.
2. There could still be other flakes lurking around, but their numbers
should definitely be going down with this change due to the increased
stability of the new AIO image.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

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
        Created At 2024-03-12 18:57:47 +0000 UTC
    </div>
</div>

