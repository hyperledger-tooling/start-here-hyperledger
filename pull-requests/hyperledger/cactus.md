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
                PR <a href="https://github.com/hyperledger/cactus/pull/969" class=".btn">#969</a>
            </td>
            <td>
                <b>
                    feat(Go-Ethereum Validator): add getNonceHex on Go-Ethereum Validator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to Issue #970 

Contents:
- (main) [Validator] add getNonce as execSyncFunction on Go-Ethereum Validator in order to solve #970.
- (sub) [car-trade] refactor to use the above function instead of web3 function.

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 14:22:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/964" class=".btn">#964</a>
            </td>
            <td>
                <b>
                    feat(aws-sm): added keychain plugin for aws secret manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Keychain</span>
            </td>
            <td>
                # Commit to be reviewed
-------------------------------
feat(aws-sm): added keychain playing for aws secret manager

        Primary Change
        ---
        1. Added new package cactus-plugin-keychain-aws-sm under packages/
        2. Added LocalStack under cactus-test-tooling/src/main/typescript for local aws secret manager deployment and testing

        Refactorings that were also necessary to incorporate 1) and 2)
        ---
        3. Updated public-api.ts under packages/cactus-test-tooling/src/main/typescript for exporting the Localstack class, its interface and constants

Resolves #912

Signed-off-by: Jagpreet Singh Sasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-13 11:56:50 +0000 UTC
    </div>
</div>

