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
                PR <a href="https://github.com/hyperledger/cactus/pull/1707" class=".btn">#1707</a>
            </td>
            <td>
                <b>
                    fix: provide generic exception handling functionality
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Introduce a log helper with static functions to get exception message /
exception stack whatever is thrown or provided.

Closes: #1702
Signed-off-by: Michael Courtin <michael.courtin@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 09:31:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1706" class=".btn">#1706</a>
            </td>
            <td>
                <b>
                    Integrate engine.io and upgrade socket.io to 3.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                engine.io is a realtime engine behind Socket.IO. It provides the foundation of a bidirectional connection between client and server

Affected versions of this package are vulnerable to Denial of Service (DoS) via a POST request to the long polling transport.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 07:03:51 +0000 UTC
    </div>
</div>

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
                <span class="chip">Corda</span><span class="chip">Tests</span>
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
                <span class="chip">Besu</span><span class="chip">Tests</span><span class="chip">Jestify</span>
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
                <span class="chip">Besu</span><span class="chip">Tests</span><span class="chip">Jestify</span>
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

