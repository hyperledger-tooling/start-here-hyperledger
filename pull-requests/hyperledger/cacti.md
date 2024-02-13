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
                PR <a href="https://github.com/hyperledger/cacti/pull/3021" class=".btn">#3021</a>
            </td>
            <td>
                <b>
                    ci(github): loosen up file matching when selecting tests to run
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Current file match glob is incorrect and never matches a file.
- I didn't find a way to filter files by extension (as it was attempted now) so I propose to loose up the rules and run the test if any file in a package has changed.

## More context
- I've noticed in another PR (https://github.com/hyperledger/cacti/pull/3018) that most tests didn't run, even though this PR changes most ts files, from all packages I think.
- I've digged a little bit in dorny/paths-filter sources, found out the file matching string is passed to `picomatch` for actual filtering.
- `picomatch` is very simple (but fast), and does not support any advanced globbing techniques. I've done some tests locally, and the best solution I found is to use less strict matching rules.

**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-12 11:10:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3020" class=".btn">#3020</a>
            </td>
            <td>
                <b>
                    build(tools): codegen clean script now removes corda kotlin-spring src
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Extended the existing globs in the clean script to include the back-end
code generated via the `kotlin-spring` template as well.

1. Previously only the generated client code was removed and regenerated
but with this change we now have the generated corda connector backend
API kotlin code removed as well.
2. The build files such as the build.gradle.kts and pom.xml files are not
deleted for now just the files under the `api` and the `model` directories
within the src/main and src/test code folders.
3. Running the delete script and then the code generation results in no
git index changes which is what we strive for.
4. The reason why we needed a slightly more complicated glob pattern
for achieving this is because the back-end code requires hand-written
implementation for the endpoints which are all placed within the `impl`
directory within the `src/main` and `src/test` folders and these need to
be ignored.
5. This change is setting the stage for an upcoming upgrade in the configuration
of the open api generator where we'll set it up to use spring boot 3 instead
of the current legacy version. The reason why this is needed is because
the legacy version has a large amount of security vulnerabilities that need
to be taken care of by upgrading our dependencies.

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
        Created At 2024-02-09 23:01:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3019" class=".btn">#3019</a>
            </td>
            <td>
                <b>
                    build(devcontainer): get git LTS from apt instead of compiling sources
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Setting the git version to LTS makes it so that the VSCode dev container feature
that we use for installing git does not fetch the source code of a specific version
and then compiles it but instead of that it just does an apt install git which has
100x faster execution time compared to the full compilation.
2. The downside of this approach is that we no longer guaranteed a specific version
of git and this could cause issues because LTS is a moving target, e.g. a form of
auto-upgrade which is something Peter's been always on a crusade against, but
trade-offs have to be made sometimes.
3. The reasoning why trade-off is appropriate is that the dev container is one of
first things that new contributors encounter/use as they ramp up with the project
and it makes a big difference if the container can be built in a few minutes vs.
a few dozen minutes.

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
        Created At 2024-02-09 21:07:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3018" class=".btn">#3018</a>
            </td>
            <td>
                <b>
                    chore(esm): change imports to esm compatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Change all relative path imports to have `.js` suffix required by the ESM standard.
- Use full import path instead of directory default import.
- I've created a tool for doing this automatically (existing tools were failing on some edge cases). The sources are available here: https://github.com/outSH/to-esm-imports.
- The tool is executed after codegen (because openapi generators doesn't support creating ESM-compatible imports yet).
- Changed jest and webpack configs to work with fully qualified ESM imports.

**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 17:48:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3017" class=".btn">#3017</a>
            </td>
            <td>
                <b>
                    build(deps): fix CVE-2024-21484 - force jsrsasign >=11.0.0 resolutions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Also upgraded the Fabric ledger related dependencies across the board
because this newer version has a higher probability of not having issues
with the newer transitive dependency that we are forcing on it.

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
        Created At 2024-02-08 23:50:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3016" class=".btn">#3016</a>
            </td>
            <td>
                <b>
                    build(deps): fix CVE-2022-25887 by upgrading sanitize-html to v2.11.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also upgraded the typings to the latest available one.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
(cherry picked from commit ad4e91bbcd216eaa36a371278a65a033698754a8)

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
        Created At 2024-02-08 23:32:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3013" class=".btn">#3013</a>
            </td>
            <td>
                <b>
                    test(cactus-core): fix false negative test results
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The fix was to start statically importing the http helper library we use
in `packages/cactus-core/src/main/typescript/web-services/handle-rest-endpoint-exception.ts`
instead of how it was (dynamic imports at runtime).

1. There have been reports of dynamic imports causing segmentation
faults in the NodeJS process when Jest is involved.
2. It is looking like this bug was another instance of that manifesting
but slightly differently because this time around Jest decided to hide
the stack trace of it as well.
3. Because of `2)` we have no specific evidence of the theory. We can only
say that the change in this commit made the problem go away, but since
there never was any crash logs or stack traces on the CI environment,
this remains a conjecture.
4. Trying to reproduce the issue locally failed even when using the
exact same versions of NodeJS and npm (and all the dependencies of course).
5. Based on `4)` it is likely that the segmentation fault is due to a
race condition in the lower level (C/C++) code of NodeJS and/or Jest.

Fixes #2966

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
        Created At 2024-02-06 23:55:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3012" class=".btn">#3012</a>
            </td>
            <td>
                <b>
                    test(cactus-core): refactor handle-rest-endpoint-exception.test.ts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change makes it easier to read and debug some of the assertions of
the test case which are a little convoluted due to the usage of the Jest
spies.

These changes were done as part of another fix but ultimately turned out
to be not a factor for that fix and therefore I thought it bess to separate
the change out onto it's own PR to make it easier to review.

Related to #2966 but this is not the actual fix.

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
        Created At 2024-02-06 23:54:40 +0000 UTC
    </div>
</div>

