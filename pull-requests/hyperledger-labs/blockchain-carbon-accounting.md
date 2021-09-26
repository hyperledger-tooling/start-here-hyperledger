---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/286" class=".btn">#286</a>
            </td>
            <td>
                <b>
                    feat(CI): add GitHub Actions pipeline for E2E tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Harsh Sharma <bcs_2019023@iiitm.ac.in>

This PR fixes #209.

Added a GitHub actions workflow to run the end-to-end tests for the project every time a new PR is opened or a new commit is pushed onto the main branch. I have followed the same setup instructions as given in the README, with the exception of uploading the seed data, as the E2E tests already account for that. However, the CI is failing in the step where the API needs to be started, as described [here](https://github.com/hyperledger-labs/blockchain-carbon-accounting/issues/209#issuecomment-927253339).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-26 08:12:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    fix queries and UI of open offsets directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 16:27:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    fix(tests): add try/catch block to tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Harsh Sharma <bcs_2019023@iiitm.ac.in>

This PR fixes #283, #80 and #190.

Added a try/catch block to the test so that even if registerAdmin fails, the rest of the tests should still run. Also, this PR removes the old tests, and so #80 and #190 become obsolete. The README.md file has also been updated with instructions on how to run the new tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 13:05:46 +0000 UTC
    </div>
</div>

