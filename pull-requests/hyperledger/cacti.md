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
                PR <a href="https://github.com/hyperledger/cacti/pull/3025" class=".btn">#3025</a>
            </td>
            <td>
                <b>
                    build(weaver/corda-driver): add Trivy scanning capability and steps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The build.gradle file now has the maven publish plugin pulled which
can be used to generate pom.xml files that we don't really plan on using
for publishing but are still necessary to have in a temporary fashion
because the scanning tool (Trivy) only suports scanning dependencies
for vulnerabilities via pom.xml files of the Maven tool but not through
`build.gradle` files of the Gradle tool.
2. The `README.md` file was updated with detailed steps on how to run a
scan that includes generating the pom file, renaming it according to the
requirements of Trivy itself and then running the actual scan.
3. Some of the cspell issues have been rectified by adding new words to
the config.

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
        Created At 2024-02-14 22:14:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3024" class=".btn">#3024</a>
            </td>
            <td>
                <b>
                    build(devcontainer): add trivy to the image specification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. This will result in the `trivy` binary being available on the path
of the dev container after a first/re-build.
2. The tool can be used to scan dependencies for versions that have
vulnerabilities.
3. The scanning has to be done a per-package basis instead of being
possible to scan the entire mono-repo in one fell swoop.
4. The documentation for the tool can be found here: https://github.com/aquasecurity/trivy

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
        Created At 2024-02-14 22:13:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3022" class=".btn">#3022</a>
            </td>
            <td>
                <b>
                    test(tools/docker): add new Corda v4.12-SNAPSHOT all-in-one image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Published on GHCR as
`ghcr.io/hyperledger/cactus-corda-4-12-all-in-one-negotiation:2024-02-13-dev`

1. It is a more bare bones flavor of the previous versions in the sense that it does not support
running the REST API web servers that come with the samples repository at all. It only supports
running the nodes A, B and Notary.
2. There is no Party C because we had to switch over to the negotiation-cordapp example.
3. This flavor of the image supports customizing the log levels of the Corda node through
the file at: tools/docker/corda-all-in-one/corda-v4_12/negotiation-cordapp/log4j2.xml
Note however that applying these changes requires a rebuild of the image so it's still less
convenient than idea lto use, but at least now we have an option to do so.
4. Another new feature of this image compared to the earlier Corda AIO images is that it
uses Ubuntu 22.04 LTS as it's base instead of alpine. This increases the image size a little
but it's well worth the trade-off of having a uniform image base (which is the long term plan)
5. There is a builder stage that can be used to clone an arbitrary branch + SHA combination of
the upstream corda git repository and then build the node .jar file from it which then will be
used by the image to run the nodes. The custom-built .jar file is placed under  /opt/bin/corda.jar
so do not mix that one up with the other one that is provided with the corda kotlin-samples repo.
6. The `run-notary-node.sh`, `run-party-a-node.sh` and `run-party-b-node.sh` scripts were altered
to use the custom-built .jar file mentioned above and this is the reason why this commit adds
a (seeming) clone of these scripts.
7. For now I did not add a CI task for building and publishing the image because even though
that would match the older images, I'm trying to save on CI resources and at the moment we
don't necessarily need a fresh build of this image on each new pull request.
8. Last but not least (first actually) this is also a security adjacent upgrade since using
this image is the precursor to a much bigger change that will see the Corda v4 connector's
dependencies upgraded to Spring Boot v3 and Corda v4.12-SNAPSHOT but we can't do that without
having this image published first if we want to have test-automation verifying those changes.

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
        Created At 2024-02-14 00:22:45 +0000 UTC
    </div>
</div>

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

