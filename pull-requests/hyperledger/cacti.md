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
                PR <a href="https://github.com/hyperledger/cacti/pull/3345" class=".btn">#3345</a>
            </td>
            <td>
                <b>
                    fix(deps): fix batch of missing production dependencies v2.0.0-rc.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Huge diff, simple changes:
1. Where applicable, I added `import type {..}` instead of `import {...}`
so that we do not need the dependency in the production dependencies.
2. For imports where the code imported was actually used at runtime I
altered the package.json file so that the dependency is marked as a production
dependency and therefore won't crash anymore when being imported in isolation
(e.g. outside of the mono-repo dev build).

Fixes #3344

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [X] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [X] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [X] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [X] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [X] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-21 01:26:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3343" class=".btn">#3343</a>
            </td>
            <td>
                <b>
                    ci: fix weaver nodejs publish ignore local .npmrc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix the issue identified in previous release, here is the error log screenshot, where it was ignoring local `.npmrc` required for publishing, and then later on `npm publish` is unable to authenticate:
<img width="1154" alt="Screenshot 2024-06-21 at 1 31 25 AM" src="https://github.com/hyperledger/cacti/assets/17192099/293d76fa-2eaf-4685-8324-3109495c56bd">
<img width="933" alt="Screenshot 2024-06-21 at 1 43 51 AM" src="https://github.com/hyperledger/cacti/assets/17192099/07f870e9-efd9-416f-b6ee-8ee2d83b8ffd">


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
        Created At 2024-06-20 20:04:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3342" class=".btn">#3342</a>
            </td>
            <td>
                <b>
                    feat(tcs-huawei-socketio): remove deprecated connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove `cactus-plugin-ledger-connector-tcs-huawei-socketio` connector and any reference to it.
- This is not permanent - we'd love to bring the package back once the necessary refactors are done!
- See issue #3155 on github for more details on context and reasoning of this decision.

Part of #3155

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
        Created At 2024-06-20 15:59:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3341" class=".btn">#3341</a>
            </td>
            <td>
                <b>
                    feat(go-ethereum-socketio): remove deprecated connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove `cactus-plugin-ledger-connector-go-ethereum-socketio` connector and any reference to it.
- Remove `SocketIOApiClient` from `cactus-api-client` since it is the last connector that was linked to it.
- Remove `legacy-socketio` option from `cactus-verifier-client`.

Part of #3155

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
        Created At 2024-06-20 15:52:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3340" class=".btn">#3340</a>
            </td>
            <td>
                <b>
                    feat(ledger-browser): refactor home page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Remove status apps, its functionality has been moved to the home page.
- Add status components for persistence apps.
- Add home page that contains cards for each configured app. Clicking on it
  naviagtes to specific app, clicking on Status button shows status component.
- Remove app drawer, replace it with a button that navigates to root path 
  (i.e. the home app, navigation between apps is handled here).
- Remove all the remaining dead and legacy code, apply small structure upgrades.
- Since this PR removes all old code, and all the current code was written by
  me and Tomasz, I've also removed previous inactive package contributors.

Depends on #3320

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
        Created At 2024-06-20 14:35:45 +0000 UTC
    </div>
</div>

