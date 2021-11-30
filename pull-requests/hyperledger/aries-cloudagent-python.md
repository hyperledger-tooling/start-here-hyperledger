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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1523" class=".btn">#1523</a>
            </td>
            <td>
                <b>
                    added documentation for wallet storage databases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - [x] SQlite
- [x] PostgreDB
- [x] Link in other documentation
- [x] Docker Compose example
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 09:46:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1521" class=".btn">#1521</a>
            </td>
            <td>
                <b>
                    Delete unused ConnRecord generated - OOB invitation  `(use_exising_connection)`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>
- resolve #1511 
- The problem it solves:
  - If 2 agents [`Alice and Bob`] have an active connection setup (using an OOB public DID invitation)
  - `Alice` send another OOB invitation (public) to `Bob`
  - `Bob` accepts it with `use_existing_connection` option, then on `Alice` side, the invitation and associated connection generated remain unused.
- ~~This PR implements `flush_stale_connections` function, which deletes all `ConnRecords` with `state: invitation` and `invitation_mode: once` which were last updated `at least 3 hours` back. The trigger for this function is creating an OOB invitation, so whenever a new `OOB invitation` is created then this cleanup is performed. Does this strategy sound reasonable?~~
- Following feedback from @swcurran, fixed initial flawed implementation of `reuse` message and used it to accomplish deletion of `hanging` connections.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 17:00:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1519" class=".btn">#1519</a>
            </td>
            <td>
                <b>
                    added logging documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added markdown documentation of logging in Acapy.

- [x] Command Line Arguments
- [x] Environment Variables
- [x] Acapy Config
- [x] Logging Config File
- [x] Link in dev readme
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 07:53:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1518" class=".btn">#1518</a>
            </td>
            <td>
                <b>
                    Fix error when removing a wallet on askar-profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes error when removing a wallet on askar-profile

### Environment
askar-profile

### Problem
Error occurred when removing a wallet.

### Fix
Unlike other options, in askar-profile, the profiles of sub wallet are not stored in `self._instances`.
However, current code always try to delete the profile in `self._instances` when removing a wallet.
This PR resolves the above problem.

Thanks!

Signed-off-by: Ethan Sung <baegjae@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 04:23:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1517" class=".btn">#1517</a>
            </td>
            <td>
                <b>
                    Fix DIF Presentation Request Input Validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1512 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 22:56:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1516" class=".btn">#1516</a>
            </td>
            <td>
                <b>
                    Fix AttributeError
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follow-up error after [PR 1515](https://github.com/hyperledger/aries-cloudagent-python/pull/1515). When calling `/credential-definitions/{cred_def_id}/write_record` in the Swagger UI, the call results in:

    AttributeError: 'IndySdkLedger' object has no attribute 'add_cred_def_non_secrets_record'

The code attempts to call `add_cred_def_non_secrets_record` on the `ledger` instance which doesn't have such a method. Instead, the actual method is in `routes.py` itself and should just be called there.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 10:43:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1515" class=".btn">#1515</a>
            </td>
            <td>
                <b>
                    Fix TypeError when calling credential_definitions_fix_cred_def_wallet…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When calling `/credential-definitions/{cred_def_id}/write_record` in the Swagger UI, the call results in a `TypeError` (same reason as in  [PR 1494](https://github.com/hyperledger/aries-cloudagent-python/pull/1494)). So the correct line of code has to be

        ledger = context.inject_or(BaseLedger)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-24 09:16:29 +0000 UTC
    </div>
</div>

