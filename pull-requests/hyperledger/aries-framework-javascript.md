---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1408" class=".btn">#1408</a>
            </td>
            <td>
                <b>
                    feat: Optionally send problem report when decline a proof request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated `declineRequest` method to acces optional `sendProblemReport` parameter indicating that Problem Report message also should be sent to Verifier.
Also updated `sendProblemReport` method to support connectionless proof request case.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 07:32:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1406" class=".btn">#1406</a>
            </td>
            <td>
                <b>
                    test(indy-vdr): add delay after DID creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In Indy VDR tests, after DID creation we are attempting to resolve the recently created DID immediately, which does not always work properly in CI. Here we add the 1000 ms delay that we also do in other Indy registrar tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-25 11:57:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1405" class=".btn">#1405</a>
            </td>
            <td>
                <b>
                    test: randomize askar wallet ids
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Randomize wallet Ids in Askar E2E tests. Also randomize Indy Postgres wallets just in case more tests are added in the future.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-25 11:09:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1403" class=".btn">#1403</a>
            </td>
            <td>
                <b>
                    test(migration): minor cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Backup now happens on the backup file, and not the original (@Vickysomtee I know you are also working on this, but it was required for the tests to be cleaned up)
- Cleaned up the tests a bit which, with a small chance, fixes some flaky CI.

Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 13:53:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1398" class=".btn">#1398</a>
            </td>
            <td>
                <b>
                    feat(core): add W3cCredentialApi
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a W3cCredentialApi class with methods for storing, removing, getting, and finding credentials and credential records.

Funded by the Ontario Government
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 12:59:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1397" class=".btn">#1397</a>
            </td>
            <td>
                <b>
                    fix: reference to indyLedgers in IndyXXXNotConfiguredError
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Errors in indy-vdr and indy-sdk were still referencing to former AgentConfig's `indyLedgers` array, which was misleading because now they are set up in module config's networks array.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 12:48:57 +0000 UTC
    </div>
</div>

