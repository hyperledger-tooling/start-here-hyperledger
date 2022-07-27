---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1870" class=".btn">#1870</a>
            </td>
            <td>
                <b>
                    Indy ledger fixes and cleanups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Move `check_existing_schema `, `create_and_send_schema` and `create_and_send_credential_definition` to the `BaseLedger` class, to avoid duplication between `IndySdkLedger` and `IndyVdrLedger` backends
- Fixes a logic error in `create_and_send_credential_definition` in `IndyVdrLedger`
- Remove unnecessary session creation in `IndySdkLedger`

I think this should resolve the most common integration test failures (published cred def not found in wallet).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 18:43:37 +0000 UTC
    </div>
</div>

