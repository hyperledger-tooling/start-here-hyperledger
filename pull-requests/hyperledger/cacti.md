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
                PR <a href="https://github.com/hyperledger/cacti/pull/3296" class=".btn">#3296</a>
            </td>
            <td>
                <b>
                    build(connector-stellar): add a run soroban transaction endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add a run soroban transaction endpoint to the Stellar Connector plugin.

**Remarks:**

The `runSorobanTransaction` endpoint can be used to make smart contract invocations on the Soroban platform. The endpoint accepts a flag called `readOnly` to indicate when the transaction should not alter ledger state. When `true`, the transaction will only be simulated based on the current ledger state and provide an up-to-date output without registering the transaction to the ledger, ensuring no fees are consumed. When `false`, the transaction will be executed and registered to the ledger even if it doesn't alter the ledger state, incurring fees as usual.

More details can be found in the `README.md` file under the connector root directory.

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
        Created At 2024-06-04 13:41:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3295" class=".btn">#3295</a>
            </td>
            <td>
                <b>
                    feat(bungee-hermes): ability to use connectors without instanciating APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BUNGEE-Hermes required API credentials for ledger connectors within its methods. This change enables using Bungee with the connectors themselves.

https://github.com/hyperledger/cacti/pull/3251#pullrequestreview-2077548976

Summary:
- This includes the implementation to possibilitate the usage of ledgers connectors without instaciating API's with bungee.
- Tests changed to test for both using connectos and API's.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-04 11:57:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3292" class=".btn">#3292</a>
            </td>
            <td>
                <b>
                    fix(security): mitigate CVE-2024-21505
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The changes made to this commit were performed by running `yarn up -R web3-utils`
in the root directory of the project which upgraded all the transitive web3-utils
dependency versions. Finally the root package.json's web3-utils declaration had
to be manually bumped as well.

Tags
- Runtime dependency
- Patch available
Weaknesses
- WeaknessCWE-1321
CVE ID
- CVE-2024-21505
GHSA ID
- GHSA-2g4c-8fpm-c46v

The security advisory:
https://github.com/hyperledger/cacti/security/dependabot/987

Related pull request that was an attempt by the robots to fix the issue (without success)
https://github.com/hyperledger/cacti/pull/3264

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
        Created At 2024-06-01 17:16:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3291" class=".btn">#3291</a>
            </td>
            <td>
                <b>
                    build(yarn): add plugin-interactive-filter to manage deps per-package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This plugin allows to resolve some CVEs more surgically that are found in indirect
dependencies which are difficult to upgrade without triggering a large change
needed and potential migrations, breaking changes to the public APIs of packages.

The reason why the above problem happens is because `yarn up` and `yarn up -R`
are blunt instruments when it comes to managing a monorepo such as ours:
They do their upgrade all-or-nothing, e.g. you can't upgrade a single dependency
in a single monorepo package, you must upgrade the dependency project-wide
with the mentioned tools, but sometimes we need to perform the upgrade just in a
single monorepo package.

For example to the above, about 20 packages use web3 but only about 5 of those
are using v4.x versions of web3. A new CVE came out covering v4.1.x and so
I needed to upgrade web3 only in those packages where web3 was already above
v4.0.0 and leave the older ones alone (surgical upgrades).

To accomplish this I've found no way to do it with stock yarn CLI commands, but
someone who had the exact same problem had written a plugin for solving it.

The original issue reported to yarn with the same problem we are having:
https://github.com/yarnpkg/berry/issues/2591

The repository where the plugin resides that we are adding in this commit in
order to remediate the problem of lack of surgical (per-package) upgrades:
https://github.com/eyolas/yarn-plugin-interractive-filter

The original CVE that I was investigating as I stumbled upon the solution:
- https://github.com/hyperledger/cacti/pull/3264
- https://github.com/hyperledger/cacti/security/dependabot/987

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
        Created At 2024-06-01 16:47:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3290" class=".btn">#3290</a>
            </td>
            <td>
                <b>
                    test(plugin-consortium-manual): fix port binding - multiple API servers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The ConnectRPC port defaults to 6000 in the API server so for test cases where multiple
instances of the API server are created and started, we need to specify the ports
explicitly in the API server config so that they don't clash with each other casusing the
test to fail.
2. The fix here was to simply bind to port 0 for all the ConnectRPC listeners which
eliminated the possibility of a clash and the test is passing once again.
3. I also snuck in a quality of life improvement for contributors: the API server will no
longer log the entire details of the fastify server that is being used for CRPC thereby
reducing the verbosity of the logs by a wide margin.

Crash logs that revealed the bug in the test case:

```sh
024-05-31T20:14:00.9554919Z [2024-05-31T20:14:00.953Z] ERROR (api-server):
Failed to start ApiServer Error: listen EADDRINUSE: address already in use 127.0.0.1:6000
2024-05-31T20:14:00.9556755Z     at Http2Server.setupListenHandle [as _listen2] (node:net:1817:16)
2024-05-31T20:14:00.9557720Z     at listenInCluster (node:net:1865:12)
2024-05-31T20:14:00.9558408Z     at doListen (node:net:2014:7)
2024-05-31T20:14:00.9559355Z     at processTicksAndRejections (node:internal/process/task_queues:83:21)
2024-05-31T20:14:00.9560500Z     at runNextTicks (node:internal/process/task_queues:64:3)
2024-05-31T20:14:00.9561451Z     at processImmediate (node:internal/timers:447:9) {
2024-05-31T20:14:00.9562333Z   code: 'EADDRINUSE',
2024-05-31T20:14:00.9562857Z   errno: -98,
2024-05-31T20:14:00.9563533Z   syscall: 'listen',
2024-05-31T20:14:00.9564068Z   address: '127.0.0.1',
2024-05-31T20:14:00.9564540Z   port: 6000
2024-05-31T20:14:00.9564959Z }
```

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
        Created At 2024-06-01 06:46:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3289" class=".btn">#3289</a>
            </td>
            <td>
                <b>
                    build: fix codegen flakiness with sequential execution, handrolled nwget
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The package.json file of the cmd-api-server package now runs the codegen related scripts
sequentially (e.g. using `run-s` instead of `run-p` of `npm-run-all`). This lowers the probability
that the download of the openapi-generator .jar file is too late to finish and a crash occurs due
to the .jar file not being present on the file-system when it is called upon.
2. Also adding a hand-built `nwget` alternative because it was hanging the process after finishing
the download (I've only seen this reproduced locally, but neveretheless it was frustrating)

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
        Created At 2024-06-01 02:17:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3288" class=".btn">#3288</a>
            </td>
            <td>
                <b>
                    chore: vendor v2.0.0-alpha.2 openapi.json files project-wide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was done by running a modified version of the bump openapi specs script.

The change ensures that there are no $ref's of type REMOTE (when an HTTP/S link is used)
present in any of the openapi.json spec files.

The upside of this change is that we can cross-reference & re-use specifications of other
packages but without the need to have the build's success depend on the internet connection
and the presence of a git tag on upstream repository (which was creating a catch-22 for
the release automation scripts).

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
        Created At 2024-06-01 02:03:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3287" class=".btn">#3287</a>
            </td>
            <td>
                <b>
                    refactor(tools): extract createTemporaryClone() utility function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This makes the tooling code a more [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)
and is a pre-requisite of some follow-up changes that are about to get proposed
in a separate pull request by Peter that are specific to vendoring the openapi.json spec files.

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
        Created At 2024-05-31 20:06:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3286" class=".btn">#3286</a>
            </td>
            <td>
                <b>
                    ci(github): fix broken ci.yaml workflow job of ethereum connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The problem seems to have been that the yarn cache restore operation
was somehow reverted to the old way of doing it which at this point
have been deprecated and broken by upgrades performed by GitHub in the
meantime.

I've updated the job definition yaml to declare the cache restore operation
the same way all the other jobs are doing it so that it doesn't crash while
attempting to restore the yarn dependency cache prior to a build+test job.

The logs of the failing job looked like this which provided the clue to
what the issue might be:

```sh
2024-05-29T18:14:26.2450767Z Current runner version: '2.316.1'
2024-05-29T18:14:26.2479056Z ##[group]Operating System
2024-05-29T18:14:26.2479698Z Ubuntu
2024-05-29T18:14:26.2480035Z 22.04.4
2024-05-29T18:14:26.2480413Z LTS
2024-05-29T18:14:26.2480746Z ##[endgroup]
2024-05-29T18:14:26.2481115Z ##[group]Runner Image
2024-05-29T18:14:26.2481603Z Image: ubuntu-22.04
2024-05-29T18:14:26.2482000Z Version: 20240526.1.0
2024-05-29T18:14:26.2482983Z Included Software: https://github.com/actions/runner-images/blob/ubuntu22/20240526.1/images/ubuntu/Ubuntu2204-Readme.md
2024-05-29T18:14:26.2484443Z Image Release: https://github.com/actions/runner-images/releases/tag/ubuntu22%2F20240526.1
2024-05-29T18:14:26.2485292Z ##[endgroup]
2024-05-29T18:14:26.2485726Z ##[group]Runner Image Provisioner
2024-05-29T18:14:26.2486244Z 2.0.369.1
2024-05-29T18:14:26.2486581Z ##[endgroup]
2024-05-29T18:14:26.2488876Z ##[group]GITHUB_TOKEN Permissions
2024-05-29T18:14:26.2490642Z Actions: write
2024-05-29T18:14:26.2491263Z Attestations: write
2024-05-29T18:14:26.2491851Z Checks: write
2024-05-29T18:14:26.2492296Z Contents: write
2024-05-29T18:14:26.2492725Z Deployments: write
2024-05-29T18:14:26.2493115Z Discussions: write
2024-05-29T18:14:26.2493536Z Issues: write
2024-05-29T18:14:26.2493922Z Metadata: read
2024-05-29T18:14:26.2494321Z Packages: write
2024-05-29T18:14:26.2494693Z Pages: write
2024-05-29T18:14:26.2495100Z PullRequests: write
2024-05-29T18:14:26.2495540Z RepositoryProjects: write
2024-05-29T18:14:26.2495985Z SecurityEvents: write
2024-05-29T18:14:26.2496416Z Statuses: write
2024-05-29T18:14:26.2496808Z ##[endgroup]
2024-05-29T18:14:26.2499861Z Secret source: Actions
2024-05-29T18:14:26.2500527Z Prepare workflow directory
2024-05-29T18:14:26.3236714Z Prepare all required actions
2024-05-29T18:14:26.3395737Z Getting action download info
2024-05-29T18:14:26.4669232Z Download action repository 'actions/setup-node@v4.0.2' (SHA:60edb5dd545a775178f52524783378180af0d1f8)
2024-05-29T18:14:26.6354890Z Download action repository 'actions/checkout@v4.1.1' (SHA:b4ffde65f46336ab88eb53be808477a3936bae11)
2024-05-29T18:14:26.6738751Z Download action repository 'actions/cache@v4.0.1' (SHA:ab5e6d0c87105b4c9c2047343972218f562e4319)
2024-05-29T18:14:26.9454684Z Complete job name: ctp-ledger-connector-ethereum
2024-05-29T18:14:27.0407144Z ##[group]Run actions/setup-node@v4.0.2
2024-05-29T18:14:27.0407904Z with:
2024-05-29T18:14:27.0408249Z   node-version: v18.18.2
2024-05-29T18:14:27.0408727Z   always-auth: false
2024-05-29T18:14:27.0409242Z   check-latest: false
2024-05-29T18:14:27.0409864Z   token: ***
2024-05-29T18:14:27.0410223Z env:
2024-05-29T18:14:27.0410660Z   NODEJS_VERSION: v18.18.2
2024-05-29T18:14:27.0411118Z   RUN_TRIVY_SCAN: true
2024-05-29T18:14:27.0411536Z   FULL_BUILD_DISABLED: true
2024-05-29T18:14:27.0412814Z   JEST_TEST_PATTERN: packages/cactus-test-plugin-ledger-connector-ethereum/src/test/typescript/(unit|integration|benchmark)/.*/*.test.ts
2024-05-29T18:14:27.0414083Z   JEST_TEST_RUNNER_DISABLED: false
2024-05-29T18:14:27.0414578Z   TAPE_TEST_RUNNER_DISABLED: true
2024-05-29T18:14:27.0415149Z ##[endgroup]
2024-05-29T18:14:27.3394142Z Attempting to download v18.18.2...
2024-05-29T18:14:27.6146256Z Acquiring 18.18.2 - x64 from https://github.com/actions/node-versions/releases/download/18.18.2-6796085386/node-18.18.2-linux-x64.tar.gz
2024-05-29T18:14:28.0584476Z Extracting ...
2024-05-29T18:14:28.0729917Z [command]/usr/bin/tar xz --strip 1 --warning=no-unknown-keyword --overwrite -C /home/runner/work/_temp/7f62dcc4-2eea-4134-9996-51fb41a608d7 -f /home/runner/work/_temp/18a8f5ad-d701-4682-a0a6-ddfeccff98bc
2024-05-29T18:14:29.0694653Z Adding to the cache ...
2024-05-29T18:14:30.6693206Z ##[group]Environment details
2024-05-29T18:14:30.9336497Z node: v18.18.2
2024-05-29T18:14:30.9337120Z npm: 9.8.1
2024-05-29T18:14:30.9337787Z yarn: 1.22.22
2024-05-29T18:14:30.9339206Z ##[endgroup]
2024-05-29T18:14:30.9702266Z ##[group]Run actions/checkout@v4.1.1
2024-05-29T18:14:30.9702711Z with:
2024-05-29T18:14:30.9703208Z   repository: hyperledger/cacti
2024-05-29T18:14:30.9704074Z   token: ***
2024-05-29T18:14:30.9704384Z   ssh-strict: true
2024-05-29T18:14:30.9704846Z   persist-credentials: true
2024-05-29T18:14:30.9705243Z   clean: true
2024-05-29T18:14:30.9705551Z   sparse-checkout-cone-mode: true
2024-05-29T18:14:30.9706019Z   fetch-depth: 1
2024-05-29T18:14:30.9706366Z   fetch-tags: false
2024-05-29T18:14:30.9706670Z   show-progress: true
2024-05-29T18:14:30.9707093Z   lfs: false
2024-05-29T18:14:30.9707406Z   submodules: false
2024-05-29T18:14:30.9707712Z   set-safe-directory: true
2024-05-29T18:14:30.9708223Z env:
2024-05-29T18:14:30.9708526Z   NODEJS_VERSION: v18.18.2
2024-05-29T18:14:30.9708865Z   RUN_TRIVY_SCAN: true
2024-05-29T18:14:30.9709297Z   FULL_BUILD_DISABLED: true
2024-05-29T18:14:30.9710676Z   JEST_TEST_PATTERN: packages/cactus-test-plugin-ledger-connector-ethereum/src/test/typescript/(unit|integration|benchmark)/.*/*.test.ts
2024-05-29T18:14:30.9711734Z   JEST_TEST_RUNNER_DISABLED: false
2024-05-29T18:14:30.9712303Z   TAPE_TEST_RUNNER_DISABLED: true
2024-05-29T18:14:30.9712669Z ##[endgroup]
2024-05-29T18:14:31.0490368Z Syncing repository: hyperledger/cacti
2024-05-29T18:14:31.0491730Z ##[group]Getting Git version info
2024-05-29T18:14:31.0492806Z Working directory is '/home/runner/work/cacti/cacti'
2024-05-29T18:14:31.0510179Z [command]/usr/bin/git version
2024-05-29T18:14:31.0595744Z git version 2.45.1
2024-05-29T18:14:31.0624616Z ##[endgroup]
2024-05-29T18:14:31.0647005Z Temporarily overriding HOME='/home/runner/work/_temp/65f40793-e9dd-45f7-aa48-3edabe0b5e12' before making global git config changes
2024-05-29T18:14:31.0648980Z Adding repository directory to the temporary git global config as a safe directory
2024-05-29T18:14:31.0650804Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/cacti/cacti
2024-05-29T18:14:31.0683363Z Deleting the contents of '/home/runner/work/cacti/cacti'
2024-05-29T18:14:31.0689073Z ##[group]Initializing the repository
2024-05-29T18:14:31.0692659Z [command]/usr/bin/git init /home/runner/work/cacti/cacti
2024-05-29T18:14:31.0791277Z hint: Using 'master' as the name for the initial branch. This default branch name
2024-05-29T18:14:31.0792241Z hint: is subject to change. To configure the initial branch name to use in all
2024-05-29T18:14:31.0793062Z hint: of your new repositories, which will suppress this warning, call:
2024-05-29T18:14:31.0793748Z hint:
2024-05-29T18:14:31.0794276Z hint: 	git config --global init.defaultBranch <name>
2024-05-29T18:14:31.0794773Z hint:
2024-05-29T18:14:31.0795453Z hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
2024-05-29T18:14:31.0796493Z hint: 'development'. The just-created branch can be renamed via this command:
2024-05-29T18:14:31.0797495Z hint:
2024-05-29T18:14:31.0798046Z hint: 	git branch -m <name>
2024-05-29T18:14:31.0798683Z Initialized empty Git repository in /home/runner/work/cacti/cacti/.git/
2024-05-29T18:14:31.0801234Z [command]/usr/bin/git remote add origin https://github.com/hyperledger/cacti
2024-05-29T18:14:31.0838315Z ##[endgroup]
2024-05-29T18:14:31.0839010Z ##[group]Disabling automatic garbage collection
2024-05-29T18:14:31.0842207Z [command]/usr/bin/git config --local gc.auto 0
2024-05-29T18:14:31.0872228Z ##[endgroup]
2024-05-29T18:14:31.0873045Z ##[group]Setting up auth
2024-05-29T18:14:31.0878799Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2024-05-29T18:14:31.0909618Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
2024-05-29T18:14:31.1265073Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2024-05-29T18:14:31.1294718Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
2024-05-29T18:14:31.1537668Z [command]/usr/bin/git config --local http.https://github.com/.extraheader AUTHORIZATION: basic ***
2024-05-29T18:14:31.1581241Z ##[endgroup]
2024-05-29T18:14:31.1582433Z ##[group]Fetching the repository
2024-05-29T18:14:31.1593800Z [command]/usr/bin/git -c protocol.version=2 fetch --no-tags --prune --no-recurse-submodules --depth=1 origin +81da3334d8e638f85e398dd228bcef836a278230:refs/remotes/origin/main
2024-05-29T18:14:32.1369829Z From https://github.com/hyperledger/cacti
2024-05-29T18:14:32.1371859Z  * [new ref]         81da3334d8e638f85e398dd228bcef836a278230 -> origin/main
2024-05-29T18:14:32.1395818Z ##[endgroup]
2024-05-29T18:14:32.1396843Z ##[group]Determining the checkout info
2024-05-29T18:14:32.1398690Z ##[endgroup]
2024-05-29T18:14:32.1399672Z ##[group]Checking out the ref
2024-05-29T18:14:32.1404086Z [command]/usr/bin/git checkout --progress --force -B main refs/remotes/origin/main
2024-05-29T18:14:32.7594778Z Switched to a new branch 'main'
2024-05-29T18:14:32.7595819Z branch 'main' set up to track 'origin/main'.
2024-05-29T18:14:32.7624017Z ##[endgroup]
2024-05-29T18:14:32.7660832Z [command]/usr/bin/git log -1 --format='%H'
2024-05-29T18:14:32.7686058Z '81da3334d8e638f85e398dd228bcef836a278230'
2024-05-29T18:14:32.7843915Z ##[group]Run echo "dir=$(yarn cache dir)" >> "$GITHUB_OUTPUT"
2024-05-29T18:14:32.7844624Z [36;1mecho "dir=$(yarn cache dir)" >> "$GITHUB_OUTPUT"[0m
2024-05-29T18:14:32.7923507Z shell: /usr/bin/bash -e {0}
2024-05-29T18:14:32.7923979Z env:
2024-05-29T18:14:32.7924456Z   NODEJS_VERSION: v18.18.2
2024-05-29T18:14:32.7924917Z   RUN_TRIVY_SCAN: true
2024-05-29T18:14:32.7925306Z   FULL_BUILD_DISABLED: true
2024-05-29T18:14:32.7926271Z   JEST_TEST_PATTERN: packages/cactus-test-plugin-ledger-connector-ethereum/src/test/typescript/(unit|integration|benchmark)/.*/*.test.ts
2024-05-29T18:14:32.7927223Z   JEST_TEST_RUNNER_DISABLED: false
2024-05-29T18:14:32.7927770Z   TAPE_TEST_RUNNER_DISABLED: true
2024-05-29T18:14:32.7928191Z ##[endgroup]
2024-05-29T18:14:33.2096065Z ##[error]Unable to process file command 'output' successfully.
2024-05-29T18:14:33.2104770Z ##[error]Invalid format '  0. yarn cache clean [--mirror] [--all]'
2024-05-29T18:14:33.2263637Z Post job cleanup.
2024-05-29T18:14:33.3035435Z [command]/usr/bin/git version
2024-05-29T18:14:33.3079712Z git version 2.45.1
2024-05-29T18:14:33.3124388Z Temporarily overriding HOME='/home/runner/work/_temp/9b8e00bb-c36a-4d67-abcb-cfafdf02bd77' before making global git config changes
2024-05-29T18:14:33.3126367Z Adding repository directory to the temporary git global config as a safe directory
2024-05-29T18:14:33.3129712Z [command]/usr/bin/git config --global --add safe.directory /home/runner/work/cacti/cacti
2024-05-29T18:14:33.3168293Z [command]/usr/bin/git config --local --name-only --get-regexp core\.sshCommand
2024-05-29T18:14:33.3203708Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'core\.sshCommand' && git config --local --unset-all 'core.sshCommand' || :"
2024-05-29T18:14:33.3479541Z [command]/usr/bin/git config --local --name-only --get-regexp http\.https\:\/\/github\.com\/\.extraheader
2024-05-29T18:14:33.3501845Z http.https://github.com/.extraheader
2024-05-29T18:14:33.3514783Z [command]/usr/bin/git config --local --unset-all http.https://github.com/.extraheader
2024-05-29T18:14:33.3547533Z [command]/usr/bin/git submodule foreach --recursive sh -c "git config --local --name-only --get-regexp 'http\.https\:\/\/github\.com\/\.extraheader' && git config --local --unset-all 'http.https://github.com/.extraheader' || :"
2024-05-29T18:14:33.4044749Z Cleaning up orphan processes
```

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
        Created At 2024-05-31 19:41:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3285" class=".btn">#3285</a>
            </td>
            <td>
                <b>
                    ci(coverage): add total typescript code coverage statistics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit** to be reviewed
---
ci(coverage): add total typescript code coverage statistics
```
Primary Changes
----------------
1. Updated the ci.yaml and ci.sh to introduce total typescript code coverage statistics using jest and istanbul-merge
```
Fixes #2661

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
        Created At 2024-05-31 06:42:24 +0000 UTC
    </div>
</div>

