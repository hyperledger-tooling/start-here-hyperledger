---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1678" class=".btn">#1678</a>
            </td>
            <td>
                <b>
                    test: jestify plugin-import-with-npm-install test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-cmd-api-server/src/test/typescript
/integration/plugin-import-with-npm-install.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana awadhana0825@gmail.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-26 22:55:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1677" class=".btn">#1677</a>
            </td>
            <td>
                <b>
                    refactor: upgrade the version of node in CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is `PR 0` that is the prerequisite for an upcoming PR that will fix issue #1654. 

What this PR does is upgrade the version in the CI from Node `v14.18.0` to Node `v16.0.0`. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-23 20:19:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1676" class=".btn">#1676</a>
            </td>
            <td>
                <b>
                    fix: add optional parameter token to CactusNode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add token to apiClient.ofLedger and PluginConsortiumManual
getConsortiumJws method when property is setted

relationed with #1579

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-22 16:17:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1672" class=".btn">#1672</a>
            </td>
            <td>
                <b>
                    test: jestify plugin-import-with-npm-install test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-cmd-api-server/src/test/typescript/
integration/plugin-import-with-npm-install.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-21 20:50:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1670" class=".btn">#1670</a>
            </td>
            <td>
                <b>
                    build: include cmd-socketio-server and socketio validators in the monorepo setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                Multiple changes, but they are tightly related to same issue so I introduced them in single PR, hope it's okay :)

- Added two build steps in common packages.json to facilitate more complex build process of packages related to this PR. I will write another comment in code to this.
- Added standalone projects to the global monorepo setup, namely:
```
./packages/cactus-cmd-socketio-server
./packages/cactus-plugin-ledger-connector-fabric-socketio
./packages/cactus-plugin-ledger-connector-go-ethereum-socketio
./packages/cactus-plugin-ledger-connector-sawtooth-socketio
```
- All changed packages extends `tsconfig.base.json`, but most overwrites strict flag to false. This is the task for another PR. After fixing strict warnings we can merge verifier tests to the main jest config.
    - Related issue - https://github.com/hyperledger/cactus/issues/1671
- All projects builds in typescript 4 set by the root config.
- Updated the README files form connectors and examples to describe new (monorepo) build process. Also converted tabs to spaces.
- I've lost a while trying to debug socketio errors when I forgot to run the init step in example app (I was sure it was my changes that caused that). I don't see for now any benefit of running two separate commands, so I've merged the init-* step to the build process itself so it's always executed.
- Rewritten socketio and go-eheterum dockerfiles. Not strictly necessary for this PR, but now they are much smaller both in dockerfile lines and resulting container size. Tested with electricty-trade - works the same as before.
- **yarn.lock update** - Changes from previous commits (I think it wasn't regenerated for a while) and from removing redundant and duplicated packages in this issue.
- Fixed bug in Verifier that caused cartrade to fail compilation - for now just restored the previous implementation. Will be part of fixes to enable strict flag in this package (another task).
- Examples were not included in monorepo setup, since it'd be tricky at the moment. It's better to containerize them instead of doing some fixes now.
- Projects use `../../.build-cache` like the other ones, so manual `npm run build` in package dir can do nothing. Do builds from root dir or clear the cache.

Closes: #1647
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-21 15:38:06 +0000 UTC
    </div>
</div>

