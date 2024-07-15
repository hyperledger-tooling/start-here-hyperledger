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
                PR <a href="https://github.com/hyperledger/cacti/pull/3388" class=".btn">#3388</a>
            </td>
            <td>
                <b>
                    test(connector-corda): fix flow-database-access-v4-8 test case 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Change:
---------------

1. The test case was broken due to a number of different issues related
to the AIO image build an also the connector image build, but on top of
those problems it also had misconfiguration issues where the port number
wasn't set to what it should be for the RPC connection that the connector
container uses to establish communications with the AIO ledger image.

Secondary Change(s):
---------------------
1. Fixed 2 bugs in the test tooling package where the port configuration
was not randomizing the exposed ports of the corda connector container and
the corda test ledger leading to accessibility issues.
2. Also introduced a createJvmInt(...) utility function on the corda connector
package which allows the flowdb test case to construct the flow invocation
requests with much less manual labor (manual coding).

In order to properly verify that this test case is working, a few other
pull requests have to be merged first and container images from those
sources published as well.

In addition to the pull request dependencies we also depend on a permission
issue being resolved in the larger GitHub organization itself as well:
https://github.com/hyperledger/governance/issues/299

Depends on #3386
Depends on #3387

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
        Created At 2024-07-08 21:19:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3387" class=".btn">#3387</a>
            </td>
            <td>
                <b>
                    feat(connector-corda): support JVM 17 Cordapps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The runner stage of the corda connector JVM image now uses an up to
date JRE instead of the very old JDK 8 which the builder stage is still
stuck on.
2. This enables the connector to load and use contract .jar files which
were built with the newer JDK as well.
3. This is important because we would like to support as wide range of
contract/flow invocation use cases as possible and also recently there's
been some changes in the Corda official samples repositories where the
contracts are being upgraded to JVM 17 as well so this will become more
and more relevant as a use-case in the near future.

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
        Created At 2024-07-08 21:09:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3386" class=".btn">#3386</a>
            </td>
            <td>
                <b>
                    test(tools): fix Corda AIO flowdb image: JVM upgrade, flow permissions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Also removed the party B, C and notary because none of these are present
in the ledger definition that we get handed down from the official kotlin
samples Corda GitHub repository.
2. The above change also saves on resources to have only party A which
makes this image boot very fast compared to the other Corda AIO images.
3. Also refactored the corda sample app enum so that the file-system paths
declared in it are matching reality instead of pointing to non-existent
directories.

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
        Created At 2024-07-08 20:28:04 +0000 UTC
    </div>
</div>

