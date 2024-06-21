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
                PR <a href="https://github.com/hyperledger/cacti/pull/3346" class=".btn">#3346</a>
            </td>
            <td>
                <b>
                    ci(custom-checks): fix depcheck not detecting missing dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                1. The depcheck tool we use have not correctly discovered some of the
missing dependencies that we have because it only verifies that the
imported dependency is present SOMEwhere in the package.json file, not that
it is specifically present in the production dependencies section which
leads to crashes and broken packages due to the API server not installing
dev dependencies when instantiating a plugin and therefore missing a few
of the dependencies that are otherwise very much needed at runtime in
production.
2. The solution to the problem was to implement our own typescript parsing
with babel and then double check the work of depcheck to make sure that
the dependencies that it marks as "no issues" are actually OK and have no
issues.
3. The hardest edge case was type imports e.g. `import type { Express } from "express";`
because the import was there, but we did not actually need that dependency
in the production dependencies as long as ALL of the imports to it in the
given package were type imports. To robustly verify this being the case or not
we had to pull out the big guns and parse all the typescript code per package
to make sure that we've looked at every single import of the dependency in
question at every single code file of the package in question.

Depends on #3345

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
        Created At 2024-06-21 01:28:21 +0000 UTC
    </div>
</div>

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3339" class=".btn">#3339</a>
            </td>
            <td>
                <b>
                    ci(release-go-sdk): use make build to test build of go-sdk
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    - chore: fix update-weaver-version script typo with quotes
    - chore: bug fix in release script go-gen-checksum

Previous release of `weaver-go-sdk` failed because of a bug in CI.
Also fixed the script `go-gen-checksum` identified in previous release and tested it on Ubuntu and Mac both.

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
        Created At 2024-06-20 08:32:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3338" class=".btn">#3338</a>
            </td>
            <td>
                <b>
                    feat(connector): remove hard dependency on keychain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Commit to be reviewed

feat(connector): remove hard dependency on keychain

    Primary Changes
    ---------------
    1. Updated besu connector to remove hard
       dependency on keychain

    Changes required to incorporate 1)
    2. Updated openapi.json file of the above mentioned connectors
       to include the new no-keychain endpoints
    3. Generated code and updated related web-services for the same

Fixes #963

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
        Created At 2024-06-20 07:22:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3337" class=".btn">#3337</a>
            </td>
            <td>
                <b>
                    build: bump the npm_and_yarn group across 35 directories with 17 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 15 updates in the / directory:

| Package | From | To |
| --- | --- | --- |
| [@grpc/grpc-js](https://github.com/grpc/grpc-node) | `1.10.3` | `1.10.9` |
| [axios](https://github.com/axios/axios) | `1.5.1` | `1.6.0` |
| [socket.io](https://github.com/socketio/socket.io) | `4.5.4` | `4.6.2` |
| [@azure/identity](https://github.com/Azure/azure-sdk-for-js) | `3.3.1` | `4.2.1` |
| [bl](https://github.com/rvagg/bl) | `5.0.0` | `5.1.0` |
| [undici](https://github.com/nodejs/undici) | `6.11.1` | `6.12.0` |
| [qs](https://github.com/ljharb/qs) | `6.7.3` | `6.8.3` |
| [vite](https://github.com/vitejs/vite/tree/HEAD/packages/vite) | `5.0.13` | `5.1.7` |
| [pkg](https://github.com/vercel/pkg) | `4.5.1` | `5.8.1` |
| [@adobe/css-tools](https://github.com/adobe/css-tools) | `4.2.0` | `4.4.0` |
| [apollo-server-core](https://github.com/apollographql/apollo-server/tree/HEAD/packages/apollo-server-core) | `3.12.0` | `3.13.0` |
| [browserify-sign](https://github.com/crypto-browserify/browserify-sign) | `4.2.1` | `4.2.3` |
| [es5-ext](https://github.com/medikoo/es5-ext) | `0.10.53` | `0.10.64` |
| [react-devtools-core](https://github.com/facebook/react/tree/HEAD/packages/react-devtools-core) | `4.27.8` | `4.28.5` |
| [word-wrap](https://github.com/jonschlinkert/word-wrap) | `1.2.3` | `1.2.5` |

Bumps the npm_and_yarn group with 4 updates in the /examples/cactus-example-discounted-asset-trade directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken), [@types/jsonwebtoken](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/HEAD/types/jsonwebtoken), [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /examples/cactus-example-electricity-trade directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 1 update in the /examples/cactus-example-electricity-trade/tools/transferNumericAsset directory: [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /examples/cactus-example-tcs-huawei directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 1 update in the /examples/cactus-example-tcs-huawei/tools/transferNumericAsset directory: [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /examples/test-run-transaction directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /extensions/cactus-plugin-htlc-coordinator-besu directory: [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /packages/cacti-plugin-ledger-connector-stellar directory: [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 3 updates in the /packages/cactus-cmd-api-server directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node), [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 3 updates in the /packages/cactus-cmd-socketio-server directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken), [@types/jsonwebtoken](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/HEAD/types/jsonwebtoken) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 1 update in the /packages/cactus-common directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node).
Bumps the npm_and_yarn group with 3 updates in the /packages/cactus-core-api directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node), [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-plugin-bungee-hermes directory: [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-plugin-keychain-azure-kv directory: [axios](https://github.com/axios/axios) and [@azure/identity](https://github.com/Azure/azure-sdk-for-js).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-plugin-ledger-connector-aries directory: [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 3 updates in the /packages/cactus-plugin-ledger-connector-besu directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node), [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-plugin-ledger-connector-ethereum directory: [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 3 updates in the /packages/cactus-plugin-ledger-connector-fabric directory: [axios](https://github.com/axios/axios), [socket.io](https://github.com/socketio/socket.io) and [bl](https://github.com/rvagg/bl).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-plugin-ledger-connector-go-ethereum-socketio directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 3 updates in the /packages/cactus-plugin-ledger-connector-iroha2 directory: [axios](https://github.com/axios/axios), [socket.io](https://github.com/socketio/socket.io) and [undici](https://github.com/nodejs/undici).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-plugin-ledger-connector-quorum directory: [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-plugin-ledger-connector-sawtooth directory: [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-plugin-ledger-connector-tcs-huawei-socketio directory: [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-plugin-persistence-ethereum directory: [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-plugin-persistence-fabric directory: [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-plugin-satp-hermes directory: [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 3 updates in the /packages/cactus-test-plugin-ledger-connector-besu directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node), [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 2 updates in the /packages/cactus-test-tooling directory: [axios](https://github.com/axios/axios) and [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 1 update in the /packages/cactus-test-verifier-client directory: [socket.io](https://github.com/socketio/socket.io).
Bumps the npm_and_yarn group with 1 update in the /weaver/common/protos-js directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node).
Bumps the npm_and_yarn group with 1 update in the /weaver/core/drivers/fabric-driver directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node).
Bumps the npm_and_yarn group with 1 update in the /weaver/core/identity-management/iin-agent directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node).
Bumps the npm_and_yarn group with 2 updates in the /weaver/samples/fabric/fabric-cli directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node) and [pkg](https://github.com/vercel/pkg).
Bumps the npm_and_yarn group with 1 update in the /weaver/sdks/fabric/interoperation-node-sdk directory: [@grpc/grpc-js](https://github.com/grpc/grpc-node).

Updates `@grpc/grpc-js` from 1.10.3 to 1.10.9
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/grpc/grpc-node/releases"><code>@​grpc/grpc-js</code>'s releases</a>.</em></p>
<blockquote>
<h2><code>@​grpc/grpc-js</code> 1.10.9</h2>
<ul>
<li>Avoid buffering significantly more than <code>grpc.max_receive_message_size</code> per received message.</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.10.8</h2>
<ul>
<li>Fix a bug that caused channels with <code>unix:</code> targets to not reconnect after the channel goes idle (<a href="https://redirect.github.com/grpc/grpc-node/issues/2750">#2750</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.10.7</h2>
<ul>
<li>Improve reporting of HTTP error codes (<a href="https://redirect.github.com/grpc/grpc-node/issues/2723">#2723</a>)</li>
<li>Update dependency on <code>@grpc/proto-loader</code> to the latest version (<a href="https://redirect.github.com/grpc/grpc-node/issues/2732">#2732</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.10.6</h2>
<ul>
<li>Fix a bug that could cause a server to sometimes send the status early (<a href="https://redirect.github.com/grpc/grpc-node/issues/2708">#2708</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.10.5</h2>
<ul>
<li>Resolve exception when <code>Error.stackTraceLimit</code> is <code>undefined</code> (<a href="https://redirect.github.com/grpc/grpc-node/issues/2701">#2701</a> contributed by <a href="https://github.com/davidfiala"><code>@​davidfiala</code></a>)</li>
<li>Call configured <code>checkServerIdentity</code> when <code>grpc.ssl_target_name_override</code> is set (<a href="https://redirect.github.com/grpc/grpc-node/issues/2704">#2704</a>)</li>
<li>Add more information to DEADLINE_EXCEEDED error details strings (<a href="https://redirect.github.com/grpc/grpc-node/issues/2692">#2692</a>)</li>
</ul>
<h2><code>@​grpc/grpc-js</code> 1.10.4</h2>
<ul>
<li>Fix a bug that caused server interceptors to crash when using partially-populated <code>ResponderBuilder</code> and <code>ListenerBuilder</code> objects (<a href="https://redirect.github.com/grpc/grpc-node/issues/2696">#2696</a>)</li>
<li>Avoid sending RST_STREAM from the client when the server has already finished its side of the stream (<a href="https://redirect.github.com/grpc/grpc-node/issues/2695">#2695</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/grpc/grpc-node/commit/674f4e351a619fd4532f84ae6dff96b8ee4e1ed3"><code>674f4e3</code></a> Merge pull request from GHSA-7v5v-9h63-cj86</li>
<li><a href="https://github.com/grpc/grpc-node/commit/7ecaa2d2dcaaa49467d41143169212caf55a40cd"><code>7ecaa2d</code></a> grpc-js: Bump to 1.10.9</li>
<li><a href="https://github.com/grpc/grpc-node/commit/e64d816d7df6d6cde62314beb67d11f1e0a8c79e"><code>e64d816</code></a> grpc-js: Avoid buffering significantly more than max_receive_message_size per...</li>
<li><a href="https://github.com/grpc/grpc-node/commit/45e5fe5462fea6cb4e3898fa2f07a4836f95916a"><code>45e5fe5</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2750">#2750</a> from murgatroid99/grpc-js_idle_uds_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/87a35414021f627f01591cade9b1f9a7dcaaf5d3"><code>87a3541</code></a> grpc-js: Fix UDS channels not reconnecting after going idle</li>
<li><a href="https://github.com/grpc/grpc-node/commit/3105791fbe8a615a28289da33ad584fb868d2ff6"><code>3105791</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2740">#2740</a> from sergiitk/backport-1.10-psm-interop-common-prod-...</li>
<li><a href="https://github.com/grpc/grpc-node/commit/fec135a9800ce884b8dd414782f4bd0014821a0c"><code>fec135a</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2729">#2729</a> from sergiitk/psm-interop-common-prod-tests</li>
<li><a href="https://github.com/grpc/grpc-node/commit/76fe802309ff39c79887d494760de25633b2beb1"><code>76fe802</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2739">#2739</a> from murgatroid99/backport-1.10-grpc-js_linkify-it_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/d5edf49f6c59fd8f6e9ead2836bc30af8284284e"><code>d5edf49</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2735">#2735</a> from murgatroid99/grpc-js_linkify-it_fix</li>
<li><a href="https://github.com/grpc/grpc-node/commit/23c05fca84cf38b9198e0010ebfe02d3ddae51a7"><code>23c05fc</code></a> Merge pull request <a href="https://redirect.github.com/grpc/grpc-node/issues/2732">#2732</a> from murgatroid99/grpc-js_proto-loader_update</li>
<li>Additional commits viewable in <a href="https://github.com/grpc/grpc-node/compare/@grpc/grpc-js@1.10.3...@grpc/grpc-js@1.10.9">compare view</a></li>
</ul>
</details>
<br />

Updates `axios` from 1.5.1 to 1.6.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>Release v1.6.0</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>CSRF:</strong> fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>) (<a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0">96ee232</a>)</li>
<li><strong>dns:</strong> fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>) (<a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8">5aaff53</a>)</li>
<li><strong>types:</strong> fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>) (<a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09">a1c8ad0</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>CVE 2023 45857 ( <a href="https://api.github.com/repos/axios/axios/pulls/6028">#6028</a> )</li>
</ul>
<pre><code>
⚠️ Critical vulnerability fix. See https://security.snyk.io/vuln/SNYK-JS-AXIOS-6032459
</code></pre>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v1.x/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h1><a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">1.6.0</a> (2023-10-26)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>CSRF:</strong> fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>) (<a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0">96ee232</a>)</li>
<li><strong>dns:</strong> fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>) (<a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8">5aaff53</a>)</li>
<li><strong>types:</strong> fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>) (<a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09">a1c8ad0</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>CVE 2023 45857 ( <a href="https://api.github.com/repos/axios/axios/pulls/6028">#6028</a> )</li>
</ul>
<pre><code>
⚠️ Critical vulnerability fix. See https://security.snyk.io/vuln/SNYK-JS-AXIOS-6032459
</code></pre>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/f7adacdbaa569281253c8cfc623ad3f4dc909c60"><code>f7adacd</code></a> chore(release): v1.6.0 (<a href="https://redirect.github.com/axios/axios/issues/6031">#6031</a>)</li>
<li><a href="https://github.com/axios/axios/commit/9917e67cbb6c157382863bad8c741de58e3f3c2b"><code>9917e67</code></a> chore(ci): fix release-it arg; (<a href="https://redirect.github.com/axios/axios/issues/6032">#6032</a>)</li>
<li><a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0"><code>96ee232</code></a> fix(CSRF): fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>)</li>
<li><a href="https://github.com/axios/axios/commit/7d45ab2e2ad6e59f5475e39afd4b286b1f393fc0"><code>7d45ab2</code></a> chore(tests): fixed tests to pass in node v19 and v20 with <code>keep-alive</code> enabl...</li>
<li><a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8"><code>5aaff53</code></a> fix(dns): fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a48a63ad823fc20e5a6a705f05f09842ca49f48c"><code>a48a63a</code></a> chore(docs): added AxiosHeaders docs; (<a href="https://redirect.github.com/axios/axios/issues/5932">#5932</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09"><code>a1c8ad0</code></a> fix(types): fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>)</li>
<li><a href="https://github.com/axios/axios/commit/2ac731d60545ba5c4202c25fd2e732ddd8297d82"><code>2ac731d</code></a> chore(docs): update readme.md (<a href="https://redirect.github.com/axios/axios/issues/5889">#5889</a>)</li>
<li>See full diff in <a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">compare view</a></li>
</ul>
</details>
<br />

Updates `socket.io` from 4.5.4 to 4.6.2
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io/releases">socket.io's releases</a>.</em></p>
<blockquote>
<h2>4.6.2</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>exports:</strong> move <code>types</code> condition to the top (<a href="https://redirect.github.com/socketio/socket.io/issues/4698">#4698</a>) (<a href="https://github.com/socketio/socket.io/commit/3d44aae381af38349fdb808d510d9f47a0c2507e">3d44aae</a>)</li>
</ul>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io/compare/4.6.1...4.6.2">https://github.com/socketio/socket.io/compare/4.6.1...4.6.2</a></li>
<li>Client release: <a href="https://github.com/socketio/socket.io-client/releases/tag/4.6.2">4.6.2</a></li>
<li><a href="https://github.com/socketio/engine.io/releases/tag/6.4.2"><code>engine.io@~6.4.2</code></a> (<a href="https://github.com/socketio/engine.io/compare/6.4.1...6.4.2">diff</a>)</li>
<li><a href="https://github.com/websockets/ws/releases/tag/8.11.0"><code>ws@~8.11.0</code></a> (no change)</li>
</ul>
<h2>4.6.1</h2>
<h3>Bug Fixes</h3>
<ul>
<li>properly handle manually created dynamic namespaces (<a href="https://github.com/socketio/socket.io/commit/0d0a7a22b5ff95f864216c529114b7dd41738d1e">0d0a7a2</a>)</li>
<li><strong>types:</strong> fix nodenext module resolution compatibility (<a href="https://redirect.github.com/socketio/socket.io/issues/4625">#4625</a>) (<a href="https://github.com/socketio/socket.io/commit/d0b22c630208669aceb7ae013180c99ef90279b0">d0b22c6</a>)</li>
</ul>
<h4>Links</h4>
<ul>
<li>Diff: <a href="https://github.com/socketio/socket.io/compare/4.6.0...4.6.1">https://github.com/socketio/socket.io/compare/4.6.0...4.6.1</a></li>
<li>Client release: <a href="https://github.com/socketio/socket.io-client/releases/tag/4.6.1">4.6.1</a></li>
<li><a href="https://github.com/socketio/engine.io/releases/tag/6.4.1"><code>engine.io@~6.4.1</code></a> (<a href="https://github.com/socketio/engine.io/compare/6.4.0...6.4.1">diff</a>)</li>
<li><a href="https://github.com/websockets/ws/releases/tag/8.11.0"><code>ws@~8.11.0</code></a> (no change)</li>
</ul>
<h2>4.6.0</h2>
<h3>Bug Fixes</h3>
<ul>
<li>add timeout method to remote socket (<a href="https://redirect.github.com/socketio/socket.io/issues/4558">#4558</a>) (<a href="https://github.com/socketio/socket.io/commit/0c0eb0016317218c2be3641e706cfaa9bea39a2d">0c0eb00</a>)</li>
<li><strong>typings:</strong> properly type emits with timeout (<a href="https://github.com/socketio/socket.io/commit/f3ada7d8ccc02eeced2b9b9ac8e4bc921eb630d2">f3ada7d</a>)</li>
</ul>
<h3>Features</h3>
<h4>Promise-based acknowledgements</h4>
<p>This commit adds some syntactic sugar around acknowledgements:</p>
<ul>
<li><code>emitWithAck()</code></li>
</ul>
<pre lang="js"><code>try {
  const responses = await io.timeout(1000).emitWithAck(&quot;some-event&quot;);
  console.log(responses); // one response per client
} catch (e) {
  // some clients did not acknowledge the event in the given delay
}
<p>io.on(&quot;connection&quot;, async (socket) =&gt; {
// without timeout
&lt;/tr&gt;&lt;/table&gt;
</code></pre></p>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/socketio/socket.io/blob/main/CHANGELOG.md">socket.io's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/socketio/socket.io/compare/4.6.1...4.6.2">4.6.2</a> (2023-05-31)</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>exports:</strong> move <code>types</code> condition to the top (<a href="https://redirect.github.com/socketio/socket.io/issues/4698">#4698</a>) (<a href="https://github.com/socketio/socket.io/commit/3d44aae381af38349fdb808d510d9f47a0c2507e">3d44aae</a>)</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github.com/socketio/engine.io/releases/tag/6.4.0"><code>engine.io@~6.4.2</code></a> (<a href="https://github.com/socketio/engine.io/compare/6.4.1...6.4.2">diff</a>)</li>
<li><a href="https://github.com/websockets/ws/releases/tag/8.11.0"><code>ws@~8.11.0</code></a> (no change)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io/compare/4.6.0...4.6.1">4.6.1</a> (2023-02-20)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>properly handle manually created dynamic namespaces (<a href="https://github.com/socketio/socket.io/commit/0d0a7a22b5ff95f864216c529114b7dd41738d1e">0d0a7a2</a>)</li>
<li><strong>types:</strong> fix nodenext module resolution compatibility (<a href="https://redirect.github.com/socketio/socket.io/issues/4625">#4625</a>) (<a href="https://github.com/socketio/socket.io/commit/d0b22c630208669aceb7ae013180c99ef90279b0">d0b22c6</a>)</li>
</ul>
<h3>Dependencies</h3>
<ul>
<li><a href="https://github.com/socketio/engine.io/releases/tag/6.4.1"><code>engine.io@~6.4.1</code></a> (<a href="https://github.com/socketio/engine.io/compare/6.4.0...6.4.1">diff</a>)</li>
<li><a href="https://github.com/websockets/ws/releases/tag/8.11.0"><code>ws@~8.11.0</code></a> (no change)</li>
</ul>
<h2><a href="https://github.com/socketio/socket.io/compare/4.5.4...4.6.0">4.6.0</a> (2023-02-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>add timeout method to remote socket (<a href="https://redirect.github.com/socketio/socket.io/issues/4558">#4558</a>) (<a href="https://github.com/socketio/socket.io/commit/0c0eb0016317218c2be3641e706cfaa9bea39a2d">0c0eb00</a>)</li>
<li><strong>typings:</strong> properly type emits with timeout (<a href="https://github.com/socketio/socket.io/commit/f3ada7d8ccc02eeced2b9b9ac8e4bc921eb630d2">f3ada7d</a>)</li>
</ul>
<h3>Features</h3>
<h4>Promise-based acknowledgements</h4>
<p>This commit adds some syntactic sugar around acknowledgements:</p>
<ul>
<li><code>emitWithAck()</code></li>
</ul>
<pre lang="js"><code>try {
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/socketio/socket.io/commit/faf914c9ab3e06a6e84fc91774a4182e58f8ae70"><code>faf914c</code></a> chore(release): 4.6.2</li>
<li><a href="https://github.com/socketio/socket.io/commit/15af22fc22bc6030fcead322c106f07640336115"><code>15af22f</code></a> refactor: add a noop handler for the error event</li>
<li><a href="https://github.com/socketio/socket.io/commit/d3658944e562e538db094ef298d274821984dea2"><code>d365894</code></a> chore: bump socket.io-parser to version 4.2.3</li>
<li><a href="https://github.com/socketio/socket.io/commit/12b0de4f524083c31b613ce33e4fd9f8d313f434"><code>12b0de4</code></a> chore: bump engine.io to version 6.4.2</li>
<li><a href="https://github.com/socketio/socket.io/commit/3d44aae381af38349fdb808d510d9f47a0c2507e"><code>3d44aae</code></a> fix(exports): move <code>types</code> condition to the top (<a href="https://redirect.github.com/socketio/socket.io/issues/4698">#4698</a>)</li>
<li><a href="https://github.com/socketio/socket.io/commit/cbf0362476a23a573233369f1119f7e305539336"><code>cbf0362</code></a> docs(examples): bump dependencies for the private messaging example</li>
<li><a href="https://github.com/socketio/socket.io/commit/59280da20b5ab6509bafb87793cc0077d60d9c27"><code>59280da</code></a> docs(examples): update examples to docker compose v2</li>
<li><a href="https://github.com/socketio/socket.io/commit/50a4d37cb82f2a14e058ae5a3038ee25796c2121"><code>50a4d37</code></a> docs(changelog): add version of transitive dependencies</li>
<li><a href="https://github.com/socketio/socket.io/commit/6458b2bef171aa0d7dea198297608ea2ed4b1db9"><code>6458b2b</code></a> docs(example): basic WebSocket-only client</li>
<li><a href="https://github.com/socketio/socket.io/commit/b56da8a99f4814d553064af175edcf747d5561d7"><code>b56da8a</code></a> docs(examples): upgrade to React 18</li>
<li>Additional commits viewable in <a href="https://github.com/socketio/socket.io/compare/4.5.4...4.6.2">compare view</a></li>
</ul>
</details>
<br />

Updates `@azure/identity` from 3.3.1 to 4.2.1
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Azure/azure-sdk-for-js/commit/183d301977d00dfd701a0bb875d5beac709dc507"><code>183d301</code></a> Upgrade to a version ESRP Release that supports federated auth (<a href="https://redirect.github.com/Azure/azure-sdk-for-js/issues/29612">#29612</a>)</li>
<li><a href="https://github.com/Azure/azure-sdk-for-js/commit/9a2afdf4fe037549527a5c83b6331218541f8f41"><code>9a2afdf</code></a> [identity] Prep for release (<a href="https://redirect.github.com/Azure/azure-sdk-for-js/issues/29981">#29981</a>)</li>
<li><a href="https://github.com/Azure/azure-sdk-for-js/commit/3caf203eb11792075e2757743501d8f95ddcc025"><code>3caf203</code></a> [identity] Prepare identity for May release (<a href="https://redirect.github.com/Azure/azure-sdk-for-js/issues/29441">#29441</a>)</li>
<li><a href="https://github.com/Azure/azure-sdk-for-js/commit/0a69729651ee312872a06ff02c7727bba77875aa"><code>0a69729</code></a> [core] CHANGELOG date for <code>@​azure-rest/core-client</code> release (<a href="https://redirect.github.com/Azure/azure-sdk-for-js/issues/29440">#29440</a>)</li>
<li><a href="https://github.com/Azure/azure-sdk-for-js/commit/88d244a809df9816ac82d19c7381f3906661e7f8"><code>88d244a</code></a> Sync eng/common directory with azure-sdk-tools for PR 8158 (<a href="https://redirect.github.com/Azure/azure-sdk-for-js/issues/29423">#29423</a>)</li>
<li><a href="https://github.com/Azure/azure-sdk-for-js/commit/77063733b075f8d1774f26ff21e6bff0bb14c981"><code>7706373</code></a> [template-dpg] Suppress build failure (<a href="https://redirect.github.com/Azure/azure-sdk-for-js/issues/29437">#29437</a>)</li>
<li><a href="https://github.com/Azure/azure-sdk-for-js/commit/769c1b126e55cf66b526f0c9e790d38cb5d4e884"><code>769c1b1</code></a> [EngSys] Update name of <code>@​azure-tools/test-utils</code>  <em><strong>NO_CI</strong></em></li>
<li><a href="https://github.com/Azure/azure-sdk-for-js/commit/8cd5bc26206bb2b47ba8310685f5271c60f2b3f0"><code>8cd5bc2</code></a> [core] New multipart/form-data primitive in core-client-rest (<a href="https://redirect.github.com/Azure/azure-sdk-for-js/issues/29047">#29047</a>)</li>
<li><a href="https://github.com/Azure/azure-sdk-for-js/commit/73b9faa5434428288cc3147817264fc1df9515a4"><code>73b9faa</code></a> [identity] Add changelog entry for MSALClient migration (<a href="https://redirect.github.com/Azure/azure-sdk-for-js/issues/29419">#29419</a>)</li>
<li><a href="https://github.com/Azure/azure-sdk-for-js/commit/b8e63a5d50f702d7bd0127cdcc92c5e3d9a9617e"><code>b8e63a5</code></a> Post release automated changes for notificationhubs releases (<a href="https://redirect.github.com/Azure/azure-sdk-for-js/issues/29431">#29431</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/Azure/azure-sdk-for-js/compare/@azure/identity_3.3.1...@azure/identity_4.2.1">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~microsoft1es">microsoft1es</a>, a new releaser for <code>@​azure/identity</code> since your current version.</p>
</details>
<br />

Updates `bl` from 5.0.0 to 5.1.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/rvagg/bl/releases">bl's releases</a>.</em></p>
<blockquote>
<h2>v5.1.0</h2>
<h2><a href="https://github.com/rvagg/bl/compare/v5.0.0...v5.1.0">5.1.0</a> (2022-10-18)</h2>
<h3>Features</h3>
<ul>
<li>added integrated TypeScript typings (<a href="https://redirect.github.com/rvagg/bl/issues/108">#108</a>) (<a href="https://github.com/rvagg/bl/commit/433ff8942f47fab8a5c9d13b2c00989ccf8d0710">433ff89</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>windows support in tests (<a href="https://github.com/rvagg/bl/commit/387dfaf9b2bca7849f12785436ceb01e42adac2c">387dfaf</a>)</li>
</ul>
<h3>Trivial Changes</h3>
<ul>
<li>GH Actions, Dependabot, auto-release, remove Travis (<a href="https://github.com/rvagg/bl/commit/997f058357de8f2a7f66998e80a72b491835573f">997f058</a>)</li>
<li><strong>no-release:</strong> bump standard from 16.0.4 to 17.0.0 (<a href="https://redirect.github.com/rvagg/bl/issues/112">#112</a>) (<a href="https://github.com/rvagg/bl/commit/078bfe33390d125297b1c946e5989c4aa9228961">078bfe3</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/rvagg/bl/blob/master/CHANGELOG.md">bl's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/rvagg/bl/compare/v5.0.0...v5.1.0">5.1.0</a> (2022-10-18)</h2>
<h3>Features</h3>
<ul>
<li>added integrated TypeScript typings (<a href="https://redirect.github.com/rvagg/bl/issues/108">#108</a>) (<a href="https://github.com/rvagg/bl/commit/433ff8942f47fab8a5c9d13b2c00989ccf8d0710">433ff89</a>)</li>
</ul>
<h3>Bug Fixes</h3>
<ul>
<li>windows support in tests (<a href="https://github.com/rvagg/bl/commit/387dfaf9b2bca7849f12785436ceb01e42adac2c">387dfaf</a>)</li>
</ul>
<h3>Trivial Changes</h3>
<ul>
<li>GH Actions, Dependabot, auto-release, remove Travis (<a href="https://github.com/rvagg/bl/commit/997f058357de8f2a7f66998e80a72b491835573f">997f058</a>)</li>
<li><strong>no-release:</strong> bump standard from 16.0.4 to 17.0.0 (<a href="https://redirect.github.com/rvagg/bl/issues/112">#112</a>) (<a href="https://github.com/rvagg/bl/commit/078bfe33390d125297b1c946e5989c4aa9228961">078bfe3</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/rvagg/bl/commit/3af8c54d33433c4683be4a74588a9739270ca4d4"><code>3af8c54</code></a> chore(release): 5.1.0 [skip ci]</li>
<li><a href="https://github.com/rvagg/bl/commit/433ff8942f47fab8a5c9d13b2c00989ccf8d0710"><code>433ff89</code></a> feat: added integrated TypeScript typings (<a href="https://redirect.github.com/rvagg/bl/issues/108">#108</a>)</li>
<li><a href="https://github.com/rvagg/bl/commit/078bfe33390d125297b1c946e5989c4aa9228961"><code>078bfe3</code></a> chore(no-release): bump standard from 16.0.4 to 17.0.0 (<a href="https://redirect.github.com/rvagg/bl/issues/112">#112</a>)</li>
<li><a href="https://github.com/rvagg/bl/commit/387dfaf9b2bca7849f12785436ceb01e42adac2c"><code>387dfaf</code></a> fix: windows support in tests</li>
<li><a href="https://github.com/rvagg/bl/commit/997f058357de8f2a7f66998e80a72b491835573f"><code>997f058</code></a> chore: GH Actions, Dependabot, auto-release, remove Travis</li>
<li>See full diff in <a href="https://github.com/rvagg/bl/compare/v5.0.0...v5.1.0">compare view</a></li>
</ul>
</details>
<br />

Updates `undici` from 6.11.1 to 6.12.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v6.12.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: broken test by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3045">nodejs/undici#3045</a></li>
<li>fix: http2 header parsing by <a href="https://github.com/climba03003"><code>@​climba03003</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3047">nodejs/undici#3047</a></li>
<li>types: fix Request.refererPolicy and RequestInit.refererPolicy are incompatible by <a href="https://github.com/zbinlin"><code>@​zbinlin</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3039">nodejs/undici#3039</a></li>
<li>fix(types): onHeaders always takes headers as an array of buffer by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3050">nodejs/undici#3050</a></li>
<li>fix: ProxyAgent causes request.headers.host to be forcibly reset by <a href="https://github.com/1zilc"><code>@​1zilc</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3026">nodejs/undici#3026</a></li>
<li>fallback to Buffer.isUtf8 on platforms without icu by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3006">nodejs/undici#3006</a></li>
<li>build(deps): bump github/codeql-action from 3.24.6 to 3.24.9 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3037">nodejs/undici#3037</a></li>
<li>build(deps): bump actions/dependency-review-action from 4.1.3 to 4.2.5 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3035">nodejs/undici#3035</a></li>
<li>build(deps): bump node from <code>577f8eb</code> to <code>87524df</code> in /build by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3055">nodejs/undici#3055</a></li>
<li>build(deps): bump node from <code>87524df</code> to <code>9696b26</code> in /build by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3058">nodejs/undici#3058</a></li>
<li>fetch: Block ports 4190 &amp; 6679 by <a href="https://github.com/KhafraDev"><code>@​KhafraDev</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3059">nodejs/undici#3059</a></li>
<li>test: activate testing for interceptors and cache by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3061">nodejs/undici#3061</a></li>
<li>cache: improve test coverage by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3063">nodejs/undici#3063</a></li>
<li>feat: modernize fuzzing by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3060">nodejs/undici#3060</a></li>
<li>fix: request abort by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3056">nodejs/undici#3056</a></li>
<li>fix: signal handling by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3053">nodejs/undici#3053</a></li>
<li>fix(H2): handle goaway properly by <a href="https://github.com/metcoder95"><code>@​metcoder95</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3057">nodejs/undici#3057</a></li>
<li>test: client, set body to null if bigger than CHUNK_LIMIT by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3064">nodejs/undici#3064</a></li>
<li>mock: improve mock interceptor by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3062">nodejs/undici#3062</a></li>
<li>fix: bad client destroy on servername change by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3066">nodejs/undici#3066</a></li>
<li>perf: improve isBlobLike by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3070">nodejs/undici#3070</a></li>
<li>test: add sanity check for llhttp wasm files by <a href="https://github.com/Uzlopak"><code>@​Uzlopak</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/3068">nodejs/undici#3068</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/zbinlin"><code>@​zbinlin</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/3039">nodejs/undici#3039</a></li>
<li><a href="https://github.com/1zilc"><code>@​1zilc</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/3026">nodejs/undici#3026</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v6.11.1...v6.12.0">https://github.com/nodejs/undici/compare/v6.11.1...v6.12.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/7751d9bcd5bbba45b60c90183aeab450b60c0831"><code>7751d9b</code></a> Bumped v6.12.0</li>
<li><a href="https://github.com/nodejs/undici/commit/e9c3b22c97b5bf2113057ea2cf1c6dec8868e9fb"><code>e9c3b22</code></a> Revert &quot;automate releases (<a href="https://redirect.github.com/nodejs/undici/issues/3052">#3052</a>)&quot;</li>
<li><a href="https://github.com/nodejs/undici/commit/f51f226522ec75a0613a07a4efc8f78938030c45"><code>f51f226</code></a> automate releases (<a href="https://redirect.github.com/nodejs/undici/issues/3052">#3052</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/502e13472d4bcebbf4669c2a91a7ef97705a0fd7"><code>502e134</code></a> test: add test for llhttp wasm (<a href="https://redirect.github.com/nodejs/undici/issues/3068">#3068</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/413fd4de5b161c1e9a539089a4d51965abd5018d"><code>413fd4d</code></a> perf: improve isBlobLike (<a href="https://redirect.github.com/nodejs/undici/issues/3070">#3070</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/7ae20e6070fa7de2831a907c92fa44268003c145"><code>7ae20e6</code></a> fix: bad client destroy on servername change (<a href="https://redirect.github.com/nodejs/undici/issues/3066">#3066</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/ad3fac577cca737976ed82cd9d55027eb8af654c"><code>ad3fac5</code></a> mock: improve mock interceptor (<a href="https://redirect.github.com/nodejs/undici/issues/3062">#3062</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/d399b3db9e16b25e9ed0f07c0e067fe99fa8c409"><code>d399b3d</code></a> test: client, set body to null if bigger than CHUNK_LIMIT (<a href="https://redirect.github.com/nodejs/undici/issues/3064">#3064</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/bc4b20698f38b4f43f0eb4091dad28c83844f3ef"><code>bc4b206</code></a> fix(H2): handle goaway properly (<a href="https://redirect.github.com/nodejs/undici/issues/3057">#3057</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/b6aa794e2db44f20adc4c9cc99009e72048f4fed"><code>b6aa794</code></a> fix: signal handling (<a href="https://redirect.github.com/nodejs/undici/issues/3053">#3053</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v6.11.1...v6.12.0">compare view</a></li>
</ul>
</details>
<br />

Updates `qs` from 6.7.3 to 6.8.3
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ljharb/qs/blob/main/CHANGELOG.md">qs's changelog</a>.</em></p>
<blockquote>
<h2><strong>6.8.3</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://redirect.github.com/ljharb/qs/issues/428">#428</a>)</li>
<li>[Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://redirect.github.com/ljharb/qs/issues/427">#427</a>)</li>
<li>[Fix] <code>stringify</code>: avoid encoding arrayformat comma when <code>encodeValuesOnly = true</code> (<a href="https://redirect.github.com/ljharb/qs/issues/424">#424</a>)</li>
<li>[readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li>[Tests] clean up stringify tests slightly</li>
<li>[Docs] add note and links for coercing primitive values (<a href="https://redirect.github.com/ljharb/qs/issues/408">#408</a>)</li>
<li>[meta] fix README.md (<a href="https://redirect.github.com/ljharb/qs/issues/399">#399</a>)</li>
<li>[actions] backport actions from main</li>
<li>[Dev Deps] backport updates from main</li>
<li>[Refactor] <code>stringify</code>: reduce branching</li>
<li>[meta] do not publish workflow files</li>
</ul>
<h2><strong>6.8.2</strong></h2>
<ul>
<li>[Fix] proper comma parsing of URL-encoded commas (<a href="https://redirect.github.com/ljharb/qs/issues/361">#361</a>)</li>
<li>[Fix] parses comma delimited array while having percent-encoded comma treated as normal text (<a href="https://redirect.github.com/ljharb/qs/issues/336">#336</a>)</li>
</ul>
<h2><strong>6.8.1</strong></h2>
<ul>
<li>[Fix] <code>parse</code>: Fix parsing array from object with <code>comma</code> true (<a href="https://redirect.github.com/ljharb/qs/issues/359">#359</a>)</li>
<li>[Fix] <code>parse</code>: throw a TypeError instead of an Error for bad charset (<a href="https://redirect.github.com/ljharb/qs/issues/349">#349</a>)</li>
<li>[Fix] <code>parse</code>: with comma true, handle field that holds an array of arrays (<a href="https://redirect.github.com/ljharb/qs/issues/335">#335</a>)</li>
<li>[fix] <code>parse</code>: with comma true, do not split non-string values (<a href="https://redirect.github.com/ljharb/qs/issues/334">#334</a>)</li>
<li>[meta] add tidelift marketing copy</li>
<li>[meta] add <code>funding</code> field</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>tape</code>, <code>safe-publish-latest</code>, <code>evalmd</code>, <code>has-symbols</code>, <code>iconv-lite</code>, <code>mkdirp</code>, <code>object-inspect</code></li>
<li>[Tests] <code>parse</code>: add passing <code>arrayFormat</code> tests</li>
<li>[Tests] use shared travis-ci configs</li>
<li>[Tests] <code>Buffer.from</code> in node v5.0-v5.9 and v4.0-v4.4 requires a TypedArray</li>
<li>[actions] add automatic rebasing / merge commit blocking</li>
</ul>
<h2><strong>6.8.0</strong></h2>
<ul>
<li>[New] add <code>depth=false</code> to preserve the original key; [Fix] <code>depth=0</code> should preserve the original key (<a href="https://redirect.github.com/ljharb/qs/issues/326">#326</a>)</li>
<li>[New] [Fix] stringify symbols and bigints</li>
<li>[Fix] ensure node 0.12 can stringify Symbols</li>
<li>[Fix] fix for an impossible situation: when the formatter is called with a non-string value</li>
<li>[Refactor] <code>formats</code>: tiny bit of cleanup.</li>
<li>[Dev Deps] update <code>eslint</code>, <code>@ljharb/eslint-config</code>, <code>browserify</code>, <code>safe-publish-latest</code>, <code>iconv-lite</code>, <code>tape</code></li>
<li>[Tests] add tests for <code>depth=0</code> and <code>depth=false</code> behavior, both current and intuitive/intended (<a href="https://redirect.github.com/ljharb/qs/issues/326">#326</a>)</li>
<li>[Tests] use <code>eclint</code> instead of <code>editorconfig-tools</code></li>
<li>[docs] readme: add security note</li>
<li>[meta] add github sponsorship</li>
<li>[meta] add FUNDING.yml</li>
<li>[meta] Clean up license text so it’s properly detected as BSD-3-Clause</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ljharb/qs/commit/0db55386013a5d92503944ad42022fd8c112c983"><code>0db5538</code></a> v6.8.3</li>
<li><a href="https://github.com/ljharb/qs/commit/639a381a66845925dba32531dcb9d21c446e9f1f"><code>639a381</code></a> [meta] do not publish workflow files</li>
<li><a href="https://github.com/ljharb/qs/commit/fc3682776670524a42e19709ec4a8138d0d7afda"><code>fc36827</code></a> [Fix] <code>parse</code>: ignore <code>__proto__</code> keys (<a href="https://redirect.github.com/ljharb/qs/issues/428">#428</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/4e312c487def80b879d5359e0d1991ce17685191"><code>4e312c4</code></a> [Robustness] <code>stringify</code>: avoid relying on a global <code>undefined</code> (<a href="https://redirect.github.com/ljharb/qs/issues/427">#427</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/57918dae411c17b232377759baaa52a642762950"><code>57918da</code></a> [Fix] <code>stringify</code>: avoid encoding arrayformat comma when `encodeValuesOnly = ...</li>
<li><a href="https://github.com/ljharb/qs/commit/48673cae0226de23f6f33cc0e17af893b42f5e37"><code>48673ca</code></a> [readme] remove travis badge; add github actions/codecov badges; update URLs</li>
<li><a href="https://github.com/ljharb/qs/commit/554ba810f1a49a25dd27c09a466490cedbee5c65"><code>554ba81</code></a> [Tests] clean up stringify tests slightly</li>
<li><a href="https://github.com/ljharb/qs/commit/dbb54a8f14573e3c7512ea01d99f75f6ce0571f8"><code>dbb54a8</code></a> [Docs] add note and links for coercing primitive values (<a href="https://redirect.github.com/ljharb/qs/issues/408">#408</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/6868128ca2bd247ba935fbb63d359d0417f6b283"><code>6868128</code></a> [meta] fix README.md (<a href="https://redirect.github.com/ljharb/qs/issues/399">#399</a>)</li>
<li><a href="https://github.com/ljharb/qs/commit/49bed6934b27c3f0ef50e1fcee8d76298d108d52"><code>49bed69</code></a> [actions] backport actions from main</li>
<li>Additional commits viewable in <a href="https://github.com/ljharb/qs/compare/v6.7.3...v6.8.3">compare view</a></li>
</ul>
</details>
<br />

Updates `vite` from 5.0.13 to 5.1.7
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/releases">vite's releases</a>.</em></p>
<blockquote>
<h2>create-vite@5.1.0</h2>
<p>Please refer to <a href="https://github.com/vitejs/vite/blob/create-vite@5.1.0/packages/create-vite/CHANGELOG.md">CHANGELOG.md</a> for details.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/blob/v5.1.7/packages/vite/CHANGELOG.md">vite's changelog</a>.</em></p>
<blockquote>
<h2><!-- raw HTML omitted -->5.1.7 (2024-03-24)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: <code>fs.deny</code> with globs with directories (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16250">#16250</a>) (<a href="https://github.com/vitejs/vite/commit/5a056dd">5a056dd</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16250">#16250</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.1.6 (2024-03-11)<!-- raw HTML omitted --></h2>
<ul>
<li>chore(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16131">#16131</a>) (<a href="https://github.com/vitejs/vite/commit/a862ecb">a862ecb</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16131">#16131</a></li>
<li>fix: check for publicDir before checking if it is a parent directory (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16046">#16046</a>) (<a href="https://github.com/vitejs/vite/commit/b6fb323">b6fb323</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16046">#16046</a></li>
<li>fix: escape single quote when relative base is used (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16060">#16060</a>) (<a href="https://github.com/vitejs/vite/commit/8f74ce4">8f74ce4</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16060">#16060</a></li>
<li>fix: handle function property extension in namespace import (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16113">#16113</a>) (<a href="https://github.com/vitejs/vite/commit/f699194">f699194</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16113">#16113</a></li>
<li>fix: server middleware mode resolve (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16122">#16122</a>) (<a href="https://github.com/vitejs/vite/commit/8403546">8403546</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16122">#16122</a></li>
<li>fix(esbuild): update tsconfck to fix bug that could cause a deadlock  (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16124">#16124</a>) (<a href="https://github.com/vitejs/vite/commit/fd9de04">fd9de04</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16124">#16124</a></li>
<li>fix(worker): hide &quot;The emitted file overwrites&quot; warning if the content is same (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16094">#16094</a>) (<a href="https://github.com/vitejs/vite/commit/60dfa9e">60dfa9e</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16094">#16094</a></li>
<li>fix(worker): throw error when circular worker import is detected and support self referencing worker (<a href="https://github.com/vitejs/vite/commit/eef9da1">eef9da1</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16103">#16103</a></li>
<li>style(utils): remove null check (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16112">#16112</a>) (<a href="https://github.com/vitejs/vite/commit/0d2df52">0d2df52</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16112">#16112</a></li>
<li>refactor(runtime): share more code between runtime and main bundle (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16063">#16063</a>) (<a href="https://github.com/vitejs/vite/commit/93be84e">93be84e</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16063">#16063</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.1.5 (2024-03-04)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: <code>__vite__mapDeps</code> code injection (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15732">#15732</a>) (<a href="https://github.com/vitejs/vite/commit/aff54e1">aff54e1</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15732">#15732</a></li>
<li>fix: analysing build chunk without dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15469">#15469</a>) (<a href="https://github.com/vitejs/vite/commit/bd52283">bd52283</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15469">#15469</a></li>
<li>fix: import with query with imports field (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16085">#16085</a>) (<a href="https://github.com/vitejs/vite/commit/ab823ab">ab823ab</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16085">#16085</a></li>
<li>fix: normalize literal-only entry pattern (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16010">#16010</a>) (<a href="https://github.com/vitejs/vite/commit/1dccc37">1dccc37</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16010">#16010</a></li>
<li>fix: optimizeDeps.entries with literal-only pattern(s) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15853">#15853</a>) (<a href="https://github.com/vitejs/vite/commit/49300b3">49300b3</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15853">#15853</a></li>
<li>fix: output correct error for empty import specifier (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16055">#16055</a>) (<a href="https://github.com/vitejs/vite/commit/a9112eb">a9112eb</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16055">#16055</a></li>
<li>fix: upgrade esbuild to 0.20.x (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16062">#16062</a>) (<a href="https://github.com/vitejs/vite/commit/899d9b1">899d9b1</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16062">#16062</a></li>
<li>fix(runtime): runtime HMR affects only imported files (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15898">#15898</a>) (<a href="https://github.com/vitejs/vite/commit/57463fc">57463fc</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15898">#15898</a></li>
<li>fix(scanner): respect  <code>experimentalDecorators: true</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15206">#15206</a>) (<a href="https://github.com/vitejs/vite/commit/4144781">4144781</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15206">#15206</a></li>
<li>revert: &quot;fix: upgrade esbuild to 0.20.x&quot; (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16072">#16072</a>) (<a href="https://github.com/vitejs/vite/commit/11cceea">11cceea</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16072">#16072</a></li>
<li>refactor: share code with vite runtime (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15907">#15907</a>) (<a href="https://github.com/vitejs/vite/commit/b20d542">b20d542</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15907">#15907</a></li>
<li>refactor(runtime): use functions from <code>pathe</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16061">#16061</a>) (<a href="https://github.com/vitejs/vite/commit/aac2ef7">aac2ef7</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16061">#16061</a></li>
<li>chore(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16028">#16028</a>) (<a href="https://github.com/vitejs/vite/commit/7cfe80d">7cfe80d</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16028">#16028</a></li>
</ul>
<h2><!-- raw HTML omitted -->5.1.4 (2024-02-21)<!-- raw HTML omitted --></h2>
<ul>
<li>perf: remove unnecessary regex s modifier (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15766">#15766</a>) (<a href="https://github.com/vitejs/vite/commit/8dc1b73">8dc1b73</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15766">#15766</a></li>
<li>fix: fs cached checks disabled by default for yarn pnp (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15920">#15920</a>) (<a href="https://github.com/vitejs/vite/commit/8b11fea">8b11fea</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15920">#15920</a></li>
<li>fix: resolve directory correctly when <code>fs.cachedChecks: true</code> (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15983">#15983</a>) (<a href="https://github.com/vitejs/vite/commit/4fe971f">4fe971f</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15983">#15983</a></li>
<li>fix: srcSet with optional descriptor (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15905">#15905</a>) (<a href="https://github.com/vitejs/vite/commit/81b3bd0">81b3bd0</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15905">#15905</a></li>
<li>fix(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15959">#15959</a>) (<a href="https://github.com/vitejs/vite/commit/571a3fd">571a3fd</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15959">#15959</a></li>
<li>fix(watch): build watch fails when outDir is empty string (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15979">#15979</a>) (<a href="https://github.com/vitejs/vite/commit/1d263d3">1d263d3</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15979">#15979</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vitejs/vite/commit/e710c2fc6d45405b5f3431bbe812abbb27946aa0"><code>e710c2f</code></a> release: v5.1.7</li>
<li><a href="https://github.com/vitejs/vite/commit/5a056dd2fc80dbafed033062fe6aaf4717309f48"><code>5a056dd</code></a> fix: <code>fs.deny</code> with globs with directories (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16250">#16250</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/6f7466e6211027686f40ad7e4ce6ec8477414546"><code>6f7466e</code></a> release: v5.1.6</li>
<li><a href="https://github.com/vitejs/vite/commit/a862ecb941a432b6e3bab62331012e4b53ddd4e8"><code>a862ecb</code></a> chore(deps): update all non-major dependencies (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16131">#16131</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/840354601a2dbdb6419429999e1f9feff31a641f"><code>8403546</code></a> fix: server middleware mode resolve (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16122">#16122</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/b6fb3235c33b1490eb0d7a33b2b62d6fa7a5496f"><code>b6fb323</code></a> fix: check for publicDir before checking if it is a parent directory (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16046">#16046</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/fd9de0473e075c8d69bb3a8867ab15300506e67b"><code>fd9de04</code></a> fix(esbuild): update tsconfck to fix bug that could cause a deadlock  (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16124">#16124</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/f6991948f59e36bc5d108e2befa5883be99f934f"><code>f699194</code></a> fix: handle function property extension in namespace import (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16113">#16113</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/0d2df527168dec95b2967a3013bbf8c1ec8b0286"><code>0d2df52</code></a> style(utils): remove null check (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16112">#16112</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/eef9da13d0028161eacc0ea699988814f29a56e4"><code>eef9da1</code></a> fix(worker): throw error when circular worker import is detected and support ...</li>
<li>Additional commits viewable in <a href="https://github.com/vitejs/vite/commits/v5.1.7/packages/vite">compare view</a></li>
</ul>
</details>
<br />

Updates `pkg` from 4.5.1 to 5.8.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vercel/pkg/releases">pkg's releases</a>.</em></p>
<blockquote>
<h2>5.8.1</h2>
<h3>Patches</h3>
<ul>
<li>Producer: properly call &quot;prebuild-install&quot; if N-API is used: dd9de59c9fca2751bf5d22b57bd9b03d43e85e80</li>
<li>Chore: clean up obsolete eslint disable comments: <a href="https://redirect.github.com/vercel/pkg/issues/1760">#1760</a></li>
<li>Chore: add prettier check in linting step: <a href="https://redirect.github.com/vercel/pkg/issues/1764">#1764</a></li>
<li>Chore: separate individual test scripts: <a href="https://redirect.github.com/vercel/pkg/issues/1759">#1759</a></li>
<li>Chore: use <code>@types/babel__generator</code> package: <a href="https://redirect.github.com/vercel/pkg/issues/1755">#1755</a></li>
<li>Chore: remove unused entry: <a href="https://redirect.github.com/vercel/pkg/issues/1766">#1766</a></li>
<li>Chore: upgrade actions runners: <a href="https://redirect.github.com/vercel/pkg/issues/1767">#1767</a></li>
<li>Style: fix typo in test-99-<a href="https://redirect.github.com/vercel/pkg/issues/1192">#1192</a>/main.js: <a href="https://redirect.github.com/vercel/pkg/issues/1790">#1790</a></li>
<li>Chore: bump prebuild-install@7.1.1: <a href="https://redirect.github.com/vercel/pkg/issues/1788">#1788</a></li>
<li>Fix: add force flag to codesign to avoid already signed error: <a href="https://redirect.github.com/vercel/pkg/issues/1756">#1756</a></li>
</ul>
<h3>Credits</h3>
<p>Huge thanks to <a href="https://github.com/ignatiusmb"><code>@​ignatiusmb</code></a>, <a href="https://github.com/eltociear"><code>@​eltociear</code></a>, <a href="https://github.com/PraveenAnaparthi"><code>@​PraveenAnaparthi</code></a>, and <a href="https://github.com/brianunlam"><code>@​brianunlam</code></a> for helping!</p>
<h2>5.8.0</h2>
<h2>Highlights</h2>
<ul>
<li>Support more language features, including but not limited to <code>classPrivateMethods</code> (<a href="https://redirect.github.com/vercel/pkg/issues/1248">#1248</a>, <a href="https://redirect.github.com/vercel/pkg/issues/1249">#1249</a>)
<ul>
<li>Note: pkg uses Babel to trace dependencies. It does NOT transform your sources. You should make sure that your code can run on the target Node.js version.</li>
</ul>
</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Bump to vercel/pkg-fetch@v3.4.2 by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1693">vercel/pkg#1693</a>
<ul>
<li>Add Node 14.20.0, 16.16.0 and 18.5.0 binaries</li>
<li><a href="https://nodejs.org/en/blog/vulnerability/july-2022-security-releases">https://nodejs.org/en/blog/vulnerability/july-2022-security-releases</a></li>
</ul>
</li>
<li>detector: use Babel AST and default plugins by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1648">vercel/pkg#1648</a></li>
<li>test: rearrange and fix order by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1650">vercel/pkg#1650</a></li>
<li>fix: typo in fabricator.ts by <a href="https://github.com/eltociear"><code>@​eltociear</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1661">vercel/pkg#1661</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/eltociear"><code>@​eltociear</code></a> made their first contribution in <a href="https://redirect.github.com/vercel/pkg/pull/1661">vercel/pkg#1661</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/vercel/pkg/compare/5.7.0...5.8.0">https://github.com/vercel/pkg/compare/5.7.0...5.8.0</a></p>
<h2>5.7.0</h2>
<h2>Highlights</h2>
<ul>
<li>Node 18 is now supported!</li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>Bump to vercel/pkg-fetch@v3.4.1 by <a href="https://github.com/jesec"><code>@​jesec</code></a> in <a href="https://redirect.github.com/vercel/pkg/pull/1616">vercel/pkg#1616</a>
<ul>
<li>No longer take NODE_OPTIONS from the environment of the end-user. Only the users (developers who use pkg to package their project) should have control over the flags via the &quot;bake in&quot; (--options) mechanism (Fixes: <a href="https://redirect.github.com/vercel/pkg/issues/954">vercel/pkg#954</a>, <a href="https://redirect.github.com/vercel/pkg/issues/989">vercel/pk...

_Description has been truncated_
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-19 16:34:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3332" class=".btn">#3332</a>
            </td>
            <td>
                <b>
                    ci(github): yarn lint job now fails if formatting was needed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If someone sends a pull request that isn't formatted according to the
tools we have in place for auto-format code (ESLint, prettier) then after
this change the CI will fail and this way we don't end up in a situation
where running `yarn lint` on the main branch produces a diff of auto-formatted
code files (which is currently sadly the case).

At the same time as introducing this constraint I'm also applying the automatic
formatting on the code project wide so that the check can actually pass as
intended when this change is getting merged.

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
        Created At 2024-06-19 00:30:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3331" class=".btn">#3331</a>
            </td>
            <td>
                <b>
                    test(connector-besu): migrate deploy-contract/* test cases to Jest
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
        Created At 2024-06-18 23:59:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3330" class=".btn">#3330</a>
            </td>
            <td>
                <b>
                    ci(github): add --ignore-scripts to lerna publish - some are failing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Longer term we'll just fix the scripts that are crashing, but right now
as a short term solution I disabled the script execution.
2. It might even be more secure for us to use this ignore scripts flag
permanently because some of the attack vectors are in those scripts which
new versions of the dependencies can execute arbitrary code.

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
        Created At 2024-06-18 16:56:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3329" class=".btn">#3329</a>
            </td>
            <td>
                <b>
                    docs(RELEASE_MANAGEMENT): explain auto-merge for release PRs is a no-no
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The detailed explanation is here:

Do not enable auto-merging on GitHub for the pull request doing the release.
The problem with auto-merging here is that it would modify the release commit's SHA as the
rebase would happen on GitHub's servers where your git signing identity is not available to use
given that GitHub does (should) not have access to your private key for signing.
The way the preserve your commit signature as valid the commit SHA must remain the same and the
way to achieve this is to perform the pull request merging with fast forward. The merging
ensures that there is no commit SHA change and the `--ff-only` option ensures that there is no
merge commit to throw a wrench in the process.

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
        Created At 2024-06-18 16:32:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3327" class=".btn">#3327</a>
            </td>
            <td>
                <b>
                    test(plugin-htlc-coordinator-besu): migrate all remaining tests to Jest
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
        Created At 2024-06-17 19:19:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3325" class=".btn">#3325</a>
            </td>
            <td>
                <b>
                    docs(goveranace): change rocketchat to discord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
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
        Created At 2024-06-17 06:45:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3324" class=".btn">#3324</a>
            </td>
            <td>
                <b>
                    chore(release): publish v2.0.0-rc.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Important** I know that there are quite a few PRs pending right now, but please do not ask to have those included in this release because that would force me to redo the entire release process from scratch. We can have subsequent v2.0.0-rc.2, v2.0.0-rc.3, v2.0.0-rc.4, etc.. releases as much as we like, but this one is particularly important to be issued ASAP because the currently "latest" version we have out on npm have dependency declaration issues that are urgently needing a fix.


# [2.0.0-rc.1](https://github.com/hyperledger/cacti/compare/v2.0.0-alpha.2...v2.0.0-rc.1) (2024-06-14)

### Bug Fixes

* **cactus-common:** coerceUnknownToError() now uses HTML sanitize ([d70488a](https://github.com/hyperledger/cacti/commit/d70488a82e9c1d6958ac3ab0368f3c3bfca378c6))
* **cactus-example-cbdc-bridging-backend:** add missing CRPC port config option ([84c0733](https://github.com/hyperledger/cacti/commit/84c0733db93e6b2cd91050c48641562130f3ea0b))
* **cmd-api-server:** add runtime type validation to HTTP verbs pulled from OAS ([b0ff599](https://github.com/hyperledger/cacti/commit/b0ff599b2c32b83d7d45c41ef215372044ccda23)), closes [#2751](https://github.com/hyperledger/cacti/issues/2751) [#2751](https://github.com/hyperledger/cacti/issues/2751) [#2751](https://github.com/hyperledger/cacti/issues/2751) [#2754](https://github.com/hyperledger/cacti/issues/2754)
* **cmd-api-server:** address CVE-2022-25881 ([81da333](https://github.com/hyperledger/cacti/commit/81da3334d8e638f85e398dd228bcef836a278230)), closes [#2862](https://github.com/hyperledger/cacti/issues/2862)
* **cmd-api-server:** fix CVE-2023-36665 protobufjs try 2 ([4e8b553](https://github.com/hyperledger/cacti/commit/4e8b5534d6a86c856768c0b47af794d66304f90d)), closes [#2682](https://github.com/hyperledger/cacti/issues/2682)
* **cmd-api-server:** healthcheck broken due to missing wget binary ([8f1ca3f](https://github.com/hyperledger/cacti/commit/8f1ca3fcce9fedaedd4ceafbb51d8e8cd41cc50e)), closes [#2894](https://github.com/hyperledger/cacti/issues/2894)
* **connector-besu:** error handling of DeployContractSolidityBytecodeEndpoint ([89d9b93](https://github.com/hyperledger/cacti/commit/89d9b93b7380477c10d8da78fcd259c95b495fa9)), closes [#2868](https://github.com/hyperledger/cacti/issues/2868)
* **connector-besu:** toBuffer only supports 0x-prefixed hex ([1d00e32](https://github.com/hyperledger/cacti/commit/1d00e32ed0f76b1d9081a7cea55ad41c956ec25b))
* **connector-corda:** contract deployment SSH reconnect race condition ([0af2eb1](https://github.com/hyperledger/cacti/commit/0af2eb13235d4dda5dfe92912be48722caea09b1))
* **connector-fabric:** address CVEs: CVE-2022-21190, CVE-2021-3918 ([11e775d](https://github.com/hyperledger/cacti/commit/11e775d6e6611d0b054cd18cca620969cb947dd8)), closes [#2864](https://github.com/hyperledger/cacti/issues/2864)
* **connector-quorum/ethereum:** strengthen contract parameter validation ([779bb7e](https://github.com/hyperledger/cacti/commit/779bb7e24b06352bad64c96eab3b24c0961d1381)), closes [#2760](https://github.com/hyperledger/cacti/issues/2760)
* **corda-simple-app:** use correct bond asset flows and contracts for bond asset exchange ([caa2b3a](https://github.com/hyperledger/cacti/commit/caa2b3a50ab7928942e72341ebc7e5511e3054f7))
* **deps:** bulk add missing dependencies - 2023-11-02 ([8addb01](https://github.com/hyperledger/cacti/commit/8addb018b6d124d54d9d948bbaeba6ea33b67153)), closes [#2857](https://github.com/hyperledger/cacti/issues/2857)
* GHSA-8qv2-5vq6-g2g7 webpki CPU denial of service in certificate path ([e24458f](https://github.com/hyperledger/cacti/commit/e24458f0541d7000ea915d97668831723744baea))
* **indy-vdr-nodejs:** update dependency version ([f81b46b](https://github.com/hyperledger/cacti/commit/f81b46bce5ca0880e6bf6b51be2233e2616759a5))
* **ledger-browser:** fix vulnerability CVE-2022-37601 ([55c7d3d](https://github.com/hyperledger/cacti/commit/55c7d3d8054af35eb903ee903a91b8f23b905998))
* **persistence-fabric:** hide not critical API ([793f94f](https://github.com/hyperledger/cacti/commit/793f94ffefe483bd2a08ad7afb30fac7aa029007))
* **plugin-htlc-coordinator-besu:** add missing HSTS header ([dff34e8](https://github.com/hyperledger/cacti/commit/dff34e8f26f94a391b8b926057cbd6346bc0b3f8))
* **plugin-keychain-vault:** fix CVE-2024-0553 in vault server image ([1eacf7e](https://github.com/hyperledger/cacti/commit/1eacf7e2a33349de794d486a47cc6bd62d93311a))
* **security:** address CVE-2021-3749 - axios >=0.22.0 ([61fc700](https://github.com/hyperledger/cacti/commit/61fc7001b1dd0849ab1d9bcab08e2475c695adae))
* **security:** mitigate CVE-2024-21505 ([f48994f](https://github.com/hyperledger/cacti/commit/f48994fe0e3736909103a844eb59cb7f3cfed247))
* **security:** remediate qs vulnerability CVE-2022-24999 ([536b6b1](https://github.com/hyperledger/cacti/commit/536b6b1b7ab9014ebcd6b162e1a467e78b52afdd))
* **weaver-asset-transfer:** return proper error messages for pledge status and claim status ([f8f6bcb](https://github.com/hyperledger/cacti/commit/f8f6bcb67733dd57b2ecde94922cff24342b7589))
* **weaver-fabric-node-sdk:** made AES key length configurable in ECIES functions ([e679801](https://github.com/hyperledger/cacti/commit/e67980141d2fb2e54ef8408e36dbab55b7195905))
* **weaver-go-cli:** updated Weaver Fabric Go CLI module to ensure local compilation ([1668cf4](https://github.com/hyperledger/cacti/commit/1668cf4104a3a653bb17ebc04d86d72b9b22547f))
* **weaver-go-sdk:** corrected membership API function signatures ([083ea4f](https://github.com/hyperledger/cacti/commit/083ea4f4464691fc967a897bf267daaeea216343))
* **weaver-go-sdk:** revert fabric-protos-go-apiv2 dep to fabric-protos-go ([6994e5b](https://github.com/hyperledger/cacti/commit/6994e5b7a43b4f3e06535babb17edd466c4d4abc))
* **weaver-membership-functions:** reverted earlier buggy change affecting identity mgmt ([faf90dd](https://github.com/hyperledger/cacti/commit/faf90ddbe9c061cd6261d642842ab12ae4be3c48))
* **weaver-packages:** removing unnecessary package-lock.json file ([f3e53e4](https://github.com/hyperledger/cacti/commit/f3e53e4625d6667a59b55647d026c59431c32d85))
* **weaver-satp:** bug and configuration fixes in relays and Fabric drivers for sample SATP implementation ([9f77871](https://github.com/hyperledger/cacti/commit/9f77871419712bacc623dd9fbbe40f6016f0a94f))
* **weaver:** improper exception handling ([a33f30c](https://github.com/hyperledger/cacti/commit/a33f30c07cb7b952581c2401da60a25170b23d1c)), closes [#2767](https://github.com/hyperledger/cacti/issues/2767)
* **weaver:** upgraded Corda dependencies to overcome Log4j vulnerability ([76f0c68](https://github.com/hyperledger/cacti/commit/76f0c680bcf74d0d78e02e95ab6c9268d15d82d2))
* **weaver:** usage of weak PRNG issue ([fa17b52](https://github.com/hyperledger/cacti/commit/fa17b52d641345a6ffc3ff6b0845be75202dc945)), closes [#2765](https://github.com/hyperledger/cacti/issues/2765)

### Features

* **actionlint:** fix the errors produced by the ActionLint tool ([e6d5d88](https://github.com/hyperledger/cacti/commit/e6d5d88fd33b2078035447bc0e452f3d862e0e68))
* **bungee-hermes:** new plugin bungee-hermes ([ecf52ec](https://github.com/hyperledger/cacti/commit/ecf52ecce310d626ea96a53c2d41dcb797510c4d))
* **bungee-hermes:** process & merge views ([231a5e5](https://github.com/hyperledger/cacti/commit/231a5e532bcb8219986dd7f5c8fa4d66cef99f34))
* **bungee-hermes:** viewProof & ethereum strategy ([22f389f](https://github.com/hyperledger/cacti/commit/22f389fc311490e5f3959b4f80e7f4caf4ac5804))
* **cactus-core-api:** add ISendRequestResultV1<T> for Fujitsu verifier ([483de38](https://github.com/hyperledger/cacti/commit/483de3838017961656c0fb850934988ae0c63c91))
* **cactus-core:** add ConnectRPC service interface and type guard ([9e83087](https://github.com/hyperledger/cacti/commit/9e830874dfed51a805566a5bedc62e3d43fc234f))
* **cactus-core:** add handleRestEndpointException utility to public API ([bf9dfe8](https://github.com/hyperledger/cacti/commit/bf9dfe882f78f7fc88ee52d86d62b7e851716b79))
* **cactus-example-discounted-asset-trade:** use openapi ethereum connector ([dcaf9fe](https://github.com/hyperledger/cacti/commit/dcaf9fe5de5b830975f3d308f140eff32d3cb79d)), closes [#2645](https://github.com/hyperledger/cacti/issues/2645)
* **cactus-example-discounted-asset-trade:** use openapi sawtooth connector ([86d6b38](https://github.com/hyperledger/cacti/commit/86d6b38e213a5304799beab48bdd46a8fc0cc0c3)), closes [#2825](https://github.com/hyperledger/cacti/issues/2825)
* **cactus-example-electricity-trade:** use openapi ethereum connector ([9e66850](https://github.com/hyperledger/cacti/commit/9e66850438c97883a8999c3def36e807bfbb1a76))
* **cactus-plugin-ledger-connector-aries:** add new connector plugin ([afef5ae](https://github.com/hyperledger/cacti/commit/afef5ae3e2f36bf7f25928ee75f82bc4800b3172)), closes [#2946](https://github.com/hyperledger/cacti/issues/2946)
* **cactus-plugin-ledger-connector-cdl-socketio:** separate endpoint for subscription key ([b1048af](https://github.com/hyperledger/cacti/commit/b1048af272e7f33fae3c68dc854d40f9be7a4e84))
* **cactus-plugin-ledger-connector-cdl-socketio:** support subscription key auth ([a04fc5b](https://github.com/hyperledger/cacti/commit/a04fc5b2593a27d5c0f9311a1ad2f83f727e2e70))
* **cactus-plugin-ledger-connector-cdl:** add new connector plugin ([6efd8de](https://github.com/hyperledger/cacti/commit/6efd8de9ff5bb8d6b894147e5c6e49aed2fa8ae4))
* **cactus-plugin-ledger-connector-ethereum:** add json-rpc proxy ([ed04201](https://github.com/hyperledger/cacti/commit/ed04201671bdb614549e995b3d88cc2cae218e56))
* **cactus-plugin-ledger-connector-ethereum:** add signing utils ([84c5b34](https://github.com/hyperledger/cacti/commit/84c5b34afa73b4f906e413c4d5dd3ff46a1dd7a8))
* **cactus-plugin-ledger-connector-ethereum:** add stress test ([55fa26e](https://github.com/hyperledger/cacti/commit/55fa26ef41d405b26da02b099418da5fa281c78f)), closes [#2631](https://github.com/hyperledger/cacti/issues/2631)
* **cactus-plugin-ledger-connector-ethereum:** refactor connector API ([cda279f](https://github.com/hyperledger/cacti/commit/cda279fb0009a4d5756c461024ad88f525bfe946)), closes [#2630](https://github.com/hyperledger/cacti/issues/2630)
* **cactus-plugin-ledger-connector-ethereum:** support London fork gas prices ([80a89dd](https://github.com/hyperledger/cacti/commit/80a89dd95d51bdc604392dbe96ab27d233b116a4)), closes [#2581](https://github.com/hyperledger/cacti/issues/2581)
* **cactus-plugin-ledger-connector-ethereum:** update web3js to 4.X ([55f82c9](https://github.com/hyperledger/cacti/commit/55f82c9568b3e875de4f3ceb89a828f8b23d65be)), closes [#2580](https://github.com/hyperledger/cacti/issues/2580) [#2535](https://github.com/hyperledger/cacti/issues/2535) [#2578](https://github.com/hyperledger/cacti/issues/2578)
* **cactus-plugin-ledger-connector-fabric-socketio:** remove fabric-socketio connector ([704e201](https://github.com/hyperledger/cacti/commit/704e201d6bd6bf7a38f0de7da60723118e18cea7)), closes [#2644](https://github.com/hyperledger/cacti/issues/2644)
* **cactus-plugin-ledger-connector-fabric:** support delegated (offline) signatures ([e2812f4](https://github.com/hyperledger/cacti/commit/e2812f4abce00a1918b8d13a6cfff382289ff998)), closes [#2598](https://github.com/hyperledger/cacti/issues/2598)
* **cactus-plugin-ledger-connector-iroha:** remove deprecated iroha connector ([fa27fde](https://github.com/hyperledger/cacti/commit/fa27fde9a28f83ff29964693be656dc107046517)), closes [#3159](https://github.com/hyperledger/cacti/issues/3159) [#3155](https://github.com/hyperledger/cacti/issues/3155)
* **cactus-plugin-ledger-connector-sawtooth:** add new connector plugin ([e379504](https://github.com/hyperledger/cacti/commit/e37950403636a3fbc378fc7462b886294e6c7923))
* **cactus-plugin-persistence-ethereum:** use openapi ethereum connector ([b8f9b79](https://github.com/hyperledger/cacti/commit/b8f9b79daa7a97cbd75325eba00c7458bfed5ce5)), closes [#2631](https://github.com/hyperledger/cacti/issues/2631)
* **cbdc-bridging:** add frontend code for the CBDC example ([5ad0ebf](https://github.com/hyperledger/cacti/commit/5ad0ebffe9de0eabbdfabb8ce8fa5c426519ee33))
* **cmd-api-server:** add ConnectRPC auto-registration for plugins ([c569460](https://github.com/hyperledger/cacti/commit/c569460b099469184a7953ffc0f806ddf3facb38))
* **cmd-api-server:** add gRPC plugin auto-registration support ([5762dad](https://github.com/hyperledger/cacti/commit/5762dadfe108c6c73251d5b474961e4888941b90))
* **common:** add express http verb method name string literal type ([8f048ea](https://github.com/hyperledger/cacti/commit/8f048ea72750595016eea4e40fd57291001cff95))
* **common:** add isGrpcStatusObjectWithCode user-defined type guard ([941dbad](https://github.com/hyperledger/cacti/commit/941dbad8fa5950b754dde97b02cc4c0ac0e9e0bb))
* **connector-besu:** add continuous benchmarking with JMeter ([379d41d](https://github.com/hyperledger/cacti/commit/379d41dd4b2cc994801c85f1fa16ea854f0301f7))
* **connector-besu:** add gRPC support for operations ([ab676d2](https://github.com/hyperledger/cacti/commit/ab676d23e1781aa17b5f2c61cb7dec643443bded)), closes [#3173](https://github.com/hyperledger/cacti/issues/3173)
* **connector-fabric:** drop support for Fabric v1.x ([ec8123c](https://github.com/hyperledger/cacti/commit/ec8123cf954b09ba8cb213c7332dfe82224c351f))
* **connector-polkadot:** add connector pkg, openapi specs, test suite ([6a476a0](https://github.com/hyperledger/cacti/commit/6a476a0f1143380d2fd6bf81c68b0842c13c6ae2))
* **core-api:** add IPluginGrpcService type & user-defined type guard ([e87e577](https://github.com/hyperledger/cacti/commit/e87e57791024824bb19830c66b9f3d2eaed6d629))
* **core:** add configureExpressAppBase() utility function ([383f852](https://github.com/hyperledger/cacti/commit/383f8528d88989b44c9763fc883c3d9ac74da21e))
* **ethereum-connector:** support block monitoring with http only connection ([f4373a9](https://github.com/hyperledger/cacti/commit/f4373a90020cbc8bfbc16da6c32babe627e7d4ae))
* **indy-sdk:** replace indy SDK with AFJ ([3291dcc](https://github.com/hyperledger/cacti/commit/3291dcc57e9e4eb04e0b9abab4134e1a5e2b0bbf)), closes [#2859](https://github.com/hyperledger/cacti/issues/2859) [#2860](https://github.com/hyperledger/cacti/issues/2860)
* **indy-test-ledger:** add helper class for indy ledger ([8c746c3](https://github.com/hyperledger/cacti/commit/8c746c331564e76e8619c5c6987cd9380ce4a13f)), closes [#2861](https://github.com/hyperledger/cacti/issues/2861)
* **plugin-keychain-memory:** add ConnectRPC support ([c5fecf6](https://github.com/hyperledger/cacti/commit/c5fecf6802efba0c982db1adc4a98b785c9cb8e0)), closes [#3183](https://github.com/hyperledger/cacti/issues/3183)
* **plugin-keychain-memory:** add observability via RxJS ReplaySubjects ([9b41377](https://github.com/hyperledger/cacti/commit/9b41377c3885cf12be3c0f49bd2745200b0d07d3))
* **plugin-keychain-memory:** add REST API endpoint implementations ([c7a8fa5](https://github.com/hyperledger/cacti/commit/c7a8fa5e3e33b3c6a1464d9762a66337176e6cdd))
* **plugin-satp-hermes:** replace IPFS dependency in SATP package ([3bb7157](https://github.com/hyperledger/cacti/commit/3bb7157b8c910c31aa3fe125ecfb3437c2bef5bb)), closes [#2984](https://github.com/hyperledger/cacti/issues/2984) [#3006](https://github.com/hyperledger/cacti/issues/3006)
* **satp:** sample implementation of SATP standard using relays ([c23197c](https://github.com/hyperledger/cacti/commit/c23197c314885b99146b52c3cd0e056439193d6e))
* **supabase-all-in-one:** update versions, use skopeo ([eeb34f9](https://github.com/hyperledger/cacti/commit/eeb34f9515bf6a7a85c1b2343b94075c4ee0a505)), closes [#3099](https://github.com/hyperledger/cacti/issues/3099)
* **test-tooling:** add Stellar test ledger ([58fa94e](https://github.com/hyperledger/cacti/commit/58fa94e194f7716934e717a0e3075773ebd31b4c)), closes [#3239](https://github.com/hyperledger/cacti/issues/3239)
* **weaver-go:** upgraded Weaver Fabric Go SDK with membership functions ([43cce8e](https://github.com/hyperledger/cacti/commit/43cce8e3778a574514d2759c282a7f0108be86b5))
* **weaver:** add build script and fix minor issues ([6d4fd00](https://github.com/hyperledger/cacti/commit/6d4fd00d457d3a72017a7cd8d4a9cf3fb4d5f37e))

### Performance Improvements

* **cmd-api-server:** add demonstration of continuous benchmarking ([0804bab](https://github.com/hyperledger/cacti/commit/0804bab4c9b43f2e22be6d77be127415a9a0532f))

### BREAKING CHANGES

* **connector-fabric:** The Open API specification that has the enums for
ledger versions will no longer have an option for Fabric v1.x
This means that in the core-api package the LedgerType enum has changes
which means that code that depends on that enum value will need to be
updated.

Fabric v1.x has had unmaintained dependencies associated with it such as
the native grpc package that stopped receiving security updates years ago
and therefore it's dangerous to have around.

There are also some issues with Fabric v1.x that make the AIO image flaky
which also makes the relevant tests flaky due to which we couldn't run
the v1.x Fabric tests on the CI for a while now anyway.

In order to reduce the CI resource usage and our own maintenance burden
I suggest that we get rid of the Fabric v1.x support meaning that we can
eliminate the AIO image build and some code complexity from the test ledger
code as well.

In addition some old fixtures can be removed that the tests were using.
Overall a net-positive as deleting code without losing functionality (that
we care about) is always a plus.

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
        Created At 2024-06-14 18:18:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3323" class=".btn">#3323</a>
            </td>
            <td>
                <b>
                    test(plugin-keychain-memory-wasm): migrate test(s) to Jest from TAP
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
        Created At 2024-06-14 17:43:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3322" class=".btn">#3322</a>
            </td>
            <td>
                <b>
                    test(connector-corda): fix flaky corda-v5-flow.test.ts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit** to be reviewed
---
test(connector-corda): fix flaky corda-v5-flow.test.ts
```
Primary Changes
----------------
1. Updated the Corda 5 aio healthcheck
2. Removed the wait time in corda-v5-flow.test.ts
```
Fixes #3293

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
        Created At 2024-06-14 09:12:33 +0000 UTC
    </div>
</div>

