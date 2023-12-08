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
                PR <a href="https://github.com/hyperledger/cacti/pull/2920" class=".btn">#2920</a>
            </td>
            <td>
                <b>
                    docs(examples): fix supply-chain-frontend run-time-error-cjs angular build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Webpack does not play nice with the `run-time-error-cjs` package's exports.
I replaced it with the vanilla `run-time-error` because the front-end
package is fine with it (does not have ESM/CJS issues like other packages)

[skip ci]

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

---

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
        Created At 2023-12-07 06:52:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2917" class=".btn">#2917</a>
            </td>
            <td>
                <b>
                    fix: GHSA-8qv2-5vq6-g2g7 webpki CPU denial of service in certificate path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                1. Upgraded tonic, prost and tokio to the latest and greatest of versions
which was necessary  because one of their transitive dependencies being
affected by the GHSA-8qv2-5vq6-g2g7 vulnerability.
2. These upgrades also forced our hand in terms of bumping up the
rust edition from 2018 to 2021 and upgrading the rust compiler to v1.74.

Depends on https://github.com/hyperledger/cacti/pull/2916 (which upgrades
the rust compiler in the dev container)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

---

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
        Created At 2023-12-06 00:46:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2916" class=".btn">#2916</a>
            </td>
            <td>
                <b>
                    build(devcontainer): upgrade rust compiler to v1.74 (current latest stable)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. This was forced through the domino effect of webpki related security
vulnerabilities that made it important for us to upgrade some dependencies
which on the other hand did not work with the slightly older rust compiler
that the dev container had had.

Relevant links for the vulnerabilities (this is not a fix yet)
- https://github.com/hyperledger/cacti/security/dependabot/762
- https://github.com/advisories/GHSA-8qv2-5vq6-g2g7

Skipping the CI because it's just a development environment change.

[skip ci]

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

---

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
        Created At 2023-12-06 00:21:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2915" class=".btn">#2915</a>
            </td>
            <td>
                <b>
                    fix(cactus-common): coerceUnknownToError() now uses HTML sanitize
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. This is a security fix so that the exception serialization does not
accidentally XSS anybody who is looking at crash logs through some
admin GUI that is designed to show logs that are considered trusted.
2. The yarn.lock file seems to have gotten out of date by accident again
so I'm also sneaking in that as an update here just to get the fix in
ASAP and without burning too much on CI execution costs.

Related discussion about `1)` can be seen at this other pull request:
https://github.com/hyperledger/cacti/pull/2893

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

---

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
        Created At 2023-12-05 22:33:21 +0000 UTC
    </div>
</div>

