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
                PR <a href="https://github.com/hyperledger/cactus/pull/1545" class=".btn">#1545</a>
            </td>
            <td>
                <b>
                    test: jestify besu-erc20 refund endpoint invalid time test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Migrated test from Tap to Jest.

File Path:
packages/cactus-test-plugin-htlc-eth-besu-erc20/src/test/typescript/integration/plugin-htlc-eth-besu-erc20/refund-endpoint-invalid-time.test.ts

This is a PARTIAL resolution to #238 and other half of test file path:
packages/cactus-test-plugin-htlc-eth-besu-erc20/src/test/typescript/integration/plugin-htlc-eth-besu-erc20/refund-endpoint.test.ts

This partially fixes #238

Signed-off-by: awadhana <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 04:00:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1544" class=".btn">#1544</a>
            </td>
            <td>
                <b>
                    feat(core-api): add weaver protocol buffer definitions #1523
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">dependencies</span><span class="chip">Core_API</span><span class="chip">P1</span><span class="chip">Weaver</span>
            </td>
            <td>
                There's two commits in this PR on purpose, one is to hold the sign-off from Rama and the other one is the admin chores performed prior to that sign-off.
This is an important milestone for us (Weaver and Cactus maintainers) working together.

---

Commit 1
---

Updated Weaver protos README and imported latest schema additions

Fixes #1523

Signed-off-by: VRamakrishna <vramakr2@in.ibm.com>

---

Commit 2
---

feat(core-api): add weaver protocol buffer definitions #1523

Adding the .proto definitions from here as discussed earlier with @VRamakrishna

To-do: I skipped the fabric driver proto due to an error on account of the
Fabric peer definitions not being present (unresolved import error).

Fixes #1523

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 23:13:55 +0000 UTC
    </div>
</div>

