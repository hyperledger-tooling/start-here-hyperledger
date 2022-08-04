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
                PR <a href="https://github.com/hyperledger/cactus/pull/2140" class=".btn">#2140</a>
            </td>
            <td>
                <b>
                    feat(iroha2-ledger): add Iroha V2 test ledger image and setup class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add a new test image for Iroha V2 (iroha2-all-in-one). It start a test ledger in single container,
  and also contains a proxy script for running iroha_client_cli.
- Add the new image to the CI.
- Add a new class for starting and interacting with Iroha V2 test ledger
  from typescript test - Iroha2TestLedger.
- Add test for test setup class to ensure basic functions are working correctly.

Relates to #2138

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 11:13:01 +0000 UTC
    </div>
</div>

