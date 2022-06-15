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
                PR <a href="https://github.com/hyperledger/cactus/pull/2078" class=".btn">#2078</a>
            </td>
            <td>
                <b>
                    feat(connector-iroha): sending transactions signed on the client-side
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add new endpoint `generate-transaction`, to create unsigned transactions
  that can be signed on the client side.
- Add a function to iroha-connector package to help signing iroha transactions
  on the client (BLP) side.
- Extend transact endpoint to accept signed transaction as an argument as well.
  New transact interface is backward compatible, all current code should work without any change.
- Add new test suite to check features implemented in this PR (i.e. signing on the client side).
- Perform minor cleanup in the connector code, remove unused fields and includes,
  fix some type related warnings.
- Perform openapi interface cleanup, format json correctly,
  mark baseConfig as required by transact (will fail otherwise),
  add error return type schemas, remove invoke-contract endpoint that was not implemented.

Closes #2077

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 15:03:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2076" class=".btn">#2076</a>
            </td>
            <td>
                <b>
                    fix: fixed lint errors pt2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed Lint errors throughout quourum-test-ledger.ts, also fixed a try catch error. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 17:39:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2075" class=".btn">#2075</a>
            </td>
            <td>
                <b>
                    fix: fixed 2 lint errors that were the any type error for Typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixed 2 lint errors that were the any type error for Typescript and removed Node

Signed-off-by: Alec Phong <alecphong@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 19:01:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2072" class=".btn">#2072</a>
            </td>
            <td>
                <b>
                    docs(build): add text build steps for Linux, Mac and Windows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Issue: #1963

Signed-off-by: Abhinav Srivastava (abhinavmir#1898 on Discord)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 02:13:32 +0000 UTC
    </div>
</div>

