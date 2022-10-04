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
                PR <a href="https://github.com/hyperledger/cactus/pull/2168" class=".btn">#2168</a>
            </td>
            <td>
                <b>
                    feat(connector-iroha2): sending transactions signed on the client-side
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                This is improvement to initial Iroha V2 PR. Please review only the last commit.

- Add new endpoint `generate-transaction`, to create unsigned transactions
  that can be signed on the client side.
- Add a function to iroha2-connector package to help signing iroha transactions
  on the client (BLP) side.
- Extend transact endpoint to accept signed transaction as an argument as well.
- Add new test suite to check features implemented in this PR (i.e. signing on the client side).

Relates to #2077

Depends on #2153

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-04 14:26:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2167" class=".btn">#2167</a>
            </td>
            <td>
                <b>
                    fix(security): vulnerabilities found in besu-all-in-one #2055
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: charelle <charelle.wrk@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-04 06:24:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2166" class=".btn">#2166</a>
            </td>
            <td>
                <b>
                    feat(connector-iroha): update-iroha-js
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                cactus-iroha plugin updated with the latest iroha-js library.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-01 12:46:45 +0000 UTC
    </div>
</div>

