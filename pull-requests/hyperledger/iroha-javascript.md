---
layout: default
title: iroha-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-javascript
---

# iroha-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/190" class=".btn">#190</a>
            </td>
            <td>
                <b>
                    [feat]: Allure reports in integration tests PoC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                This PR introduces a foundation for further development of [Compatibility Matrix](https://hyperledger.github.io/iroha-2-docs/reference/compatibility-matrix.html) tests.

The main places for them is among all Client Node.js integration tests (`packages/client/test/integration/test-node`). When these tests run, `allure-reports` directory is generated (in the tests directory).

Additionally, in this PR I refactor tests structure in general, making it easier to maintain and expand them.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-08 09:51:03 +0000 UTC
    </div>
</div>

