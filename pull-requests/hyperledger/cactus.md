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
                PR <a href="https://github.com/hyperledger/cactus/pull/2174" class=".btn">#2174</a>
            </td>
            <td>
                <b>
                    Move inactive maintainers to emeritus status
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The TOC approved a requirement that maintainers
that have not been active in over three to six
months be move to emeritus status.

These maintainers have not been active in over
one year.

hyperledger/toc#32

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 18:31:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2173" class=".btn">#2173</a>
            </td>
            <td>
                <b>
                    chore(release): publish v1.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also manually changing the "publishConfig" property of the
packages/cactus-cmd-socketio-server/package.json
file because it was not set to public which excluded it from the
release automation altogether in previous releases, causing this bug
to be reported:
https://github.com/hyperledger/cactus/issues/2069

Fixes #2069

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 18:00:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2172" class=".btn">#2172</a>
            </td>
            <td>
                <b>
                    feat(connector-iroha2): sending queries signed on the client-side
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Add new helper method for signing query payload on the client side.
- Change `query` and `generateTransaction` to support both query and transaction payload generation and
  sending.
- Refactor `CactusIrohaV2QueryClient` to return query context instead of single request method.
- Update tests to fit the new API.
- Add tests for signing queries on the client side.

Depends on https://github.com/hyperledger/cactus/pull/2171

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 12:40:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2171" class=".btn">#2171</a>
            </td>
            <td>
                <b>
                    feat(connector-iroha2): wait for transaction commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Add a new argument to transact endpoint to wait for transaction commit. When this flag is true, request will return with final transaction status (commit / reject).
- Add new transaction hash to all the responses from the transact endpoint.
- Alter tests to wait for status instead of waiting for X seconds to make them more reliable.
- Add new tests to check this PR features.

Relates to https://github.com/hyperledger/cactus/issues/2077

Depends on https://github.com/hyperledger/cactus/pull/2168

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 14:42:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2170" class=".btn">#2170</a>
            </td>
            <td>
                <b>
                    Fixing the broken vs-code badge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Kamal Nayan <95926324+legendarykamal@users.noreply.github.com>

Solves #2169
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 10:26:48 +0000 UTC
    </div>
</div>

