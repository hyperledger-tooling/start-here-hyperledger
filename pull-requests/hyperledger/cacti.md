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
                PR <a href="https://github.com/hyperledger/cacti/pull/3382" class=".btn">#3382</a>
            </td>
            <td>
                <b>
                    feat(satp-hermes): Fabric and Besu Bridges POC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bridges POC

- Test for Besu and Fabric Implementation
- Besu and Fabric Contracts (ERC20 example and the wrapper contract)

closes [#3281](https://github.com/hyperledger/cacti/issues/3281)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-04 12:49:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3380" class=".btn">#3380</a>
            </td>
            <td>
                <b>
                    docs(examples): migrate supply chain app to XDai connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                1. We are in the process of decomissioning the Quorum connector and this
is a pre-requisite to that end.

Depends on #3379
> test(test-tooling): fix BesuTestLedger start cfg: publish all ports)

Fixes #3272

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
        Created At 2024-07-04 02:42:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3379" class=".btn">#3379</a>
            </td>
            <td>
                <b>
                    test(test-tooling): fix BesuTestLedger start cfg: publish all ports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Previously we specified the publish all ports flag of the Docker Engine
incorrectly and this lead to the ports not actually being published on
randomized ports.
2. This broke the supply chain app example when we tried to migrate it to
use 2 separate besu test ledger instances in tandem because they were
conflicting on the ports due to the lack of randomization.

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
        Created At 2024-07-04 02:31:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3378" class=".btn">#3378</a>
            </td>
            <td>
                <b>
                    build(docs/examples): add yarn patch to @ionic deps of example frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                1. The `main` field of the package.json of these two packages were invalid
because the `main` field was set to `bundle.js` but that file is actually
under `ngx/bundle.js` within the package directory and therefore the value
of it originally was invalid that caused warnings in our tooling.
2. By using the yarn **patch** feature we overcame this problem by modifying
the sources of the dependencies in question: `@ionic-native/splash-screen` and
`@ionic-native/status-bar`

Depends on https://github.com/lerna-lite/lerna-lite/pull/887

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
        Created At 2024-07-03 23:43:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3377" class=".btn">#3377</a>
            </td>
            <td>
                <b>
                    chore(release): publish v2.0.0-rc.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
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
        Created At 2024-07-03 22:42:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3376" class=".btn">#3376</a>
            </td>
            <td>
                <b>
                    test(common): jest migration of the key-converter utility test cases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The problem was that the database schema was defined in a way that was
destroying timestamp information during insertion of records.
2. Updating the schema to hold the timestamp information made the test pass.

More information about why it's recommended to store datetime data with
the TIMESTAMPTZ column type is explained by the author of the node-postgres
library which is an important part of the problem (it assumes local time
for columns that do not store the timestamp time zone).

https://node-postgres.com/features/types#date--timestamp--timestamptz

Fixes #3373

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
        Created At 2024-07-03 22:10:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3375" class=".btn">#3375</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): use ncc bundle in container image - CVE-2024-29415
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes the CVE mentioned and also improves our response time to future CVEs
by a very wide margin. Details below.

1. Fixing the mentioned vulnerability in the API server and doing so in
a way so that in the future our dependency upgrades automatically propagate
to the container builds as well.
2. The way we are achieving this is by making the container image build
use the pre-built bundle instead of pulling the package contents from npm.
3. This has the advantage of breaking the chicken egg problem with releases
to npm and container images, so from now on if we are adding a fix to the
API server in the code, the built container image will automatically contain
that fix when building on the CI for the pull request.
4. This is also a new pattern for how to create our container images that
has a couple more improvements to it:
4.1. The .dockerignore file is now specific to the particular package's
container image instead of the global one in the project root being used.
This was needed because we are copying files from the ./dist/ folder of the
package to the container image at build time but this was not possible while
the root dir .dockerignore file was in effect because it blanket ignores
the ./dist/ folders overall and so the image building was failing with errors
that it couldn't locate the bundle (which is inside the ./dist/ directory)
4.2. The healthcheck of the container is now 100% self-contained and needs
no external dependencies of any kind (neither npm nor operating system level ones)
This is beneficial because it reduces the attack-surface of the image and also
reduce the size of the image by at least a 100 MB.
4.3. With the introduction of the usage of the bundled version of the code
we have **dramatically** reduced the image size overall. The image built from
this revision of the code is 221 MB while the previous image versions were
hovering closer to a 0.5 GB.
5. Also updated the README of the package so that all the examples pertaining
to the container image are now fully functional once again.
6. Simplified the container image's definition: the custom docker entrypoint
script and the healthcheck bash script are no longer necessary.
7. Renamed the container image definition file from `Dockerfile` to
`cmd-api-server.Dockerfile` because this is mandated by Docker when building
images with custom .dockerignore files (it needs the custom filename to
disambiguate the .dockerignore files based on it)
8. Refactored how the CI executes the Trivy scan to reduce resource usage:
8.1. There is no separate image build job now. This was necessary because
with the new image definition we have to have the project compiled first
(since we no longer install directly from npm) so it would've been a lot of
duplicated compute time to recompile the project in yet another CI job for the
image build.

The image built from this revision is also published on the official repository
with the canary tag of:
`ghcr.io/hyperledger/cactus-cmd-api-server:2024-07-03T19-32-51-dev-3f5e97893`

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
        Created At 2024-07-03 19:38:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3374" class=".btn">#3374</a>
            </td>
            <td>
                <b>
                    fix(plugin-persistence-ethereum): make created_at TIMESTAMPTZ in schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The problem was that the database schema was defined in a way that was
destroying timestamp information during insertion of records.
2. Updating the schema to hold the timestamp information made the test pass.

More information about why it's recommended to store datetime data with
the TIMESTAMPTZ column type is explained by the author of the node-postgres
library which is an important part of the problem (it assumes local time
for columns that do not store the timestamp time zone).

https://node-postgres.com/features/types#date--timestamp--timestamptz

Fixes #3373

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
        Created At 2024-07-02 19:41:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3372" class=".btn">#3372</a>
            </td>
            <td>
                <b>
                    chore(weaver): use docker compose v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `Primary change:  Updates the weaver files
to use docker compose v2 syntax.  docker-compose
v1 will be dropped on the github runners
shortly.`

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
        Created At 2024-07-02 14:06:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3370" class=".btn">#3370</a>
            </td>
            <td>
                <b>
                    chore(cleanup): deleted deprecated files and folders
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Deleted 'docs-cactus' and 'weaver/docs' folders.
- Ensured that the latest contents in the above are reflected in the 'docs' folder.
- Updated MAINTAINERS.md file with contents from 'weaver/MAINTAINERS.md'.
- Deleted unnecessary 'MAINTAINERS.md' and 'CONTRIBUTING.md' in the 'weaver' folder.
- Fixed indentations and removed dead code in source files.

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
        Created At 2024-07-01 19:06:57 +0000 UTC
    </div>
</div>

