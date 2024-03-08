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
                PR <a href="https://github.com/hyperledger/cacti/pull/3048" class=".btn">#3048</a>
            </td>
            <td>
                <b>
                    style(docs/examples/supply-chain): move block scoped code to functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a purely stylistic change that makes the code read much better
and also reduces the chance of future bugs that would get introduced due
to block scoping side effects that people not experienced with the
language could make.

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
        Created At 2024-03-02 02:47:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3047" class=".btn">#3047</a>
            </td>
            <td>
                <b>
                    refactor(test-tooling): fix types of streams: use NodeJS.ReadableStream
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The container management library that we use in the test infrastructure
(called dockerode) is expecting streams that are defined in the global
namespace of the `@types/node` library, e.g. the standard library of NodeJS
itself.
2. Previously we were using the "streams" package to provide type information
to the streams that we were passing around to dockerode and it was working
fine, but after some changes that seem unrelated this has broken the
compilation process.
3. The mentioned changes are not yet on the main branch, but we expect
them to be there soon and so this change is laying the groundwork for that
by pre-emptively fixing the broken build's root cause which is that the
test-tooling package does not declare it's typings related dependencies
correctly: It implicitly uses the NodeJS standard library's types but
so far had not declared them on the package level.
4. This change is therefore to rectify the issue of the `@types/node`
dependency missing from the test-tooling package and also the refactoring
of some of the test ledger classes which were relying on the `streams`
builtin package instead of correctly using the NodeJS.ReadableStream global.
5. Earlier the reasoning for this was that we try to avoid pulling in
types from the global scope because we try to avoid any sort of dependency
on the global scope in general. Once we have proof though that this is
causing issues with the build, then we must give up the principle for
practical reasons (and only in the minimum viable scope, e.g. this does
not change the fact that everywhere else in the codebase we should still
do our best to avoid using the global scoped classes, types, functions,
etc..).

Thank you to @AndreAugusto11 and @RafaelAPB for pointing out this issue
through the pull request of his that is currently being worked on at the
time of this writing:
https://github.com/RafaelAPB/blockchain-integration-framework/pull/72

Related to but does not address #2811

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
        Created At 2024-03-01 19:04:18 +0000 UTC
    </div>
</div>

