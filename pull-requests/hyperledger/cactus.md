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
                PR <a href="https://github.com/hyperledger/cactus/pull/2153" class=".btn">#2153</a>
            </td>
            <td>
                <b>
                    feat(connector-iroha2): add support for Iroha V2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Add new Iroha V2 cactus connector.
- Two OpenAPI endpoints are implemented: `transact` and `query`. Both endpoints support
  critical subset of instructions and queries supported by the upstream javascript iroha sdk.
- One SocketIO endpoint can be used to monitor new blocks from the ledger.
- New connector can be used through a verifier-client interface.
- All added functions are tested in functional test suites and documented.
- Added execution of Iroha2 tests to the CI.

Additional notes:
- Connector doesn't work well with cactus module system, the issue has been reported and described
  in README. PR is not merge-ready until this is fixed (the CI should fail now).
- Iroha V2 javascript packages are not available on official npm yet, had to include `.npmrc` with
  private npm address. I'm not sure if there's ETA of delivering these through NPM, so it might be
  necessary to commit it after all.

Closes #2138
Depends on #2140

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 14:59:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2152" class=".btn">#2152</a>
            </td>
            <td>
                <b>
                    fix(cactus-example-electricity-trade): enable tsconfig strict flag an…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …d fix all the warnings

Fixed all warnings when strict flag is enabled

Closes: #2144

Signed-off-by: Tomasz Awramski <tomasz.awramski@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 09:29:13 +0000 UTC
    </div>
</div>

