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
                PR <a href="https://github.com/hyperledger/cacti/pull/2861" class=".btn">#2861</a>
            </td>
            <td>
                <b>
                    feat(indy-sdk): replace indy SDK with AFJ
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Refactor test ledger `indy-testnet` into `indy-all-in-one`. New package uses
    the latest indy version, has healtcheck script, updated startup / cleanup
    scripts.
- Remove `indy-sdk-cli` image since it's not used anymore.
- Refactor `cactus-example-discounted-asset-trade` to use own aries agent
    instead of indy connector. This way it doesn't need to use indy-sdk anymore,
    and python indy connector can be safely removed / upgraded.
- Update sample app readme to explain current workflow.
- Remove client scripts since `cactus-example-discounted-asset-trade-client`
    can now be used to interact with the sample app.
- Add `cactus-example-discounted-asset-trade-client`. It contains script for
    setting up test credentials on the ledger, script with interactive menu for
    interacting with `cactus-example-discounted-asset-trade` sample app,
    and bunch of helper functions used for writing these apps.

Depends on #2859
Depends on #2860

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

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
        Created At 2023-11-03 20:30:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2859" class=".btn">#2859</a>
            </td>
            <td>
                <b>
                    fix(deps): bulk add missing dependencies - 2023-11-02
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Added missing dependencies everywhere to all the packages
2. The exception to the above is test runners and related dependencies.
You can see the detailed exclusion list in the source code of the script
itself [1]. We should make these configurable later on as well. For
reference, this is what the exclusions were declared as when I ran the
tool in order to then proceed to update the package.json files:

```typescript
ignorePatterns: [
    // files matching these patterns will be ignored
    "sandbox",
    "dist",
    "bower_components",
    "node_modules"
],
ignoreMatches: [
    // ignore dependencies that matches these globs
    "grunt-*",
    "jest-extended",
    "tape-promise",
    "tape",
    "tap",
    "@ionic-native/*"
],
```
3. There were instances of missing dependency usages where we did NOT
have to add the dependencies to package.json files because what we could
do instead is just import types at development time by using the
`import type { .. } from "...";`  syntax of Typescript which means that
the import is disappeared during transpilation completely. So this is why
some source code files were also modified and not strictly just package.json
files.
4. Added a script in the ./tools/custom-check directory to audit the
entire mono-repo for missing NodeJS dependencies.

We've had at least a dozen packages that were missing production
dependency declarations from their package.json files. The usual suspects
here are packages that are contained by the root node_modules folder
which masks the problem at development time (e.g. the compiler won't
let you know about the missing dependencies).

For a future-proof solution we should add a commit hook or other validation
that runs the custom check that I added [2] here to verify that there are no
missing dependencies in the project

[1] `./tools/custom-checks/check-missing-node-deps.ts`
[2] `$ yarn tools:check-missing-node-deps`

Fixes #2857

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
        Created At 2023-11-02 21:19:17 +0000 UTC
    </div>
</div>

