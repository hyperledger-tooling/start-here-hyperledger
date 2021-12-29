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
                PR <a href="https://github.com/hyperledger/cactus/pull/1701" class=".btn">#1701</a>
            </td>
            <td>
                <b>
                    test(test-tooling): add corda 5 aio image #1479
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #1479 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-29 09:55:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1700" class=".btn">#1700</a>
            </td>
            <td>
                <b>
                    test: jestify get-single-status-endpoint test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu-erc20/src/
test/typescript/integration/plugin-htlc-eth-besu-erc20/
get-single-status-endpoint.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-29 01:47:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1699" class=".btn">#1699</a>
            </td>
            <td>
                <b>
                    test: jestify refund-endpoint test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu/
src/test/typescript/integration/
plugin-htlc-eth-besu/refund-endpoint.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-29 00:16:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1696" class=".btn">#1696</a>
            </td>
            <td>
                <b>
                    build(socket.io, socket.io-client): upgrade to common socket.io version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">dependent</span>
            </td>
            <td>
                Some packages use socket.io and socket.io-client V2, while other use V4.
In order for these components to communicate, we must use common
socket.io version in all cactus packages (V4.1.3). This commit introduce
some other related changes, like merging socketio unit tests to common
setup (to assert changes are correct) and fixes some strict-flag
warnings and minor bugs. It also updates python packages requirements
and updates readme when it was necessary.

Closes: #1679
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

Additional changes in **cactus-cmd-socketio-server**:
- Removed local jest config, test will be run from the root dir now.
- Fixed several strict flag warnings from verifier component.
- Removed nohoist pragma, changed package to public and added license info.
- Added monitor_error handle to fix few unit tests (cherry-picked from #1660)
- Used common socketio test helpers (cherry-picked from #1660)

**Depends on #1670**
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 17:18:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1695" class=".btn">#1695</a>
            </td>
            <td>
                <b>
                    test: jestify withdraw-endpoint test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu/src/
test/typescript/integration/plugin-htlc-eth-besu/
withdraw-endpoint.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 04:30:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1694" class=".btn">#1694</a>
            </td>
            <td>
                <b>
                    test: jestify initialize-endpoint test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu-erc20/
src/test/typescript/integration/
plugin-htlc-eth-besu-erc20/initialize-endpoint.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 04:23:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1693" class=".btn">#1693</a>
            </td>
            <td>
                <b>
                    test: jestify refund-endpoint-invalid test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu/
src/test/typescript/integration/
plugin-htlc-eth-besu/refund-endpoint-invalid.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 04:10:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1692" class=".btn">#1692</a>
            </td>
            <td>
                <b>
                    test: jestify get-status-endpoint-invalid test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu/src/
test/typescript/integration/plugin-htlc-eth-besu/
get-status-endpoint-invalid.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 04:01:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1691" class=".btn">#1691</a>
            </td>
            <td>
                <b>
                    test: jestify get-status-endpoint test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu/
src/test/typescript/integration/
plugin-htlc-eth-besu/get-status-endpoint.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 03:46:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1689" class=".btn">#1689</a>
            </td>
            <td>
                <b>
                    test: jestify get-single-status-endpoint-invalid test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu/src/
test/typescript/integration/plugin-htlc-eth-besu/
get-single-status-endpoint-invalid.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 03:11:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1688" class=".btn">#1688</a>
            </td>
            <td>
                <b>
                    test: jestify new-contract-endpoint-invalid test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu/src/
test/typescript/integration/plugin-htlc-eth-besu/
new-contract-endpoint-invalid.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 02:15:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1687" class=".btn">#1687</a>
            </td>
            <td>
                <b>
                    test: jestify new-contract-endpoint test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu/src/
test/typescript/integration/plugin-htlc-eth-besu/
new-contract-endpoint.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 02:04:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1686" class=".btn">#1686</a>
            </td>
            <td>
                <b>
                    test: jestify js-object-signer test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-common/src/test/typescript/
unit/js-object-signer.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 01:51:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1685" class=".btn">#1685</a>
            </td>
            <td>
                <b>
                    test: jestify get-node-jws-endpoint-v1 test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-plugin-consortium-manual/src/test/
typescript/unit/consortium/get-node-jws-endpoint-v1.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 01:44:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1683" class=".btn">#1683</a>
            </td>
            <td>
                <b>
                    ci: ensure sorted json files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Please do not mind this PR, I've been working on this issue and it's been really fickle so I am testing it to see what the problem is. So sorry about the pings! 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-27 19:52:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1682" class=".btn">#1682</a>
            </td>
            <td>
                <b>
                    test: jestify initialize-endpoint test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span><span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu/src
/test/typescript/integration/plugin-htlc-eth-besu
/initialize-endpoint.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-27 19:36:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1681" class=".btn">#1681</a>
            </td>
            <td>
                <b>
                    test: jestify initialize-endpoint-invalid test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu/src/
test/typescript/integration/plugin-htlc-eth-besu/
initialize-endpoint-invalid.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-27 17:42:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1680" class=".btn">#1680</a>
            </td>
            <td>
                <b>
                    test: jestify jwt-endpoint-authorization test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Tests</span><span class="chip">Jestify</span>
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-cmd-api-server/src/test/
typescript/integration/jwt-endpoint-authorization.test.ts

This is a PARTIAL resolution to issue #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-27 17:20:03 +0000 UTC
    </div>
</div>

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

