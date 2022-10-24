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
                PR <a href="https://github.com/hyperledger/cactus/pull/2178" class=".btn">#2178</a>
            </td>
            <td>
                <b>
                    feat(connector-iroha2): add more iroha v2 tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Add test for complex scenario that involves creating new account and asset, and then transferring assets between two accounts.
- Add test for parsing retrieved block data to find specific transaction hashes.

Depends on https://github.com/hyperledger/cactus/pull/2172

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

Please review only the last commit.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 15:18:48 +0000 UTC
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

