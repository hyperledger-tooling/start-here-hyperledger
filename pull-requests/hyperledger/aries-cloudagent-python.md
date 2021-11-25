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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1510" class=".btn">#1510</a>
            </td>
            <td>
                <b>
                    Fix bug when getting credentials on askar-profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes bug when getting credentials under askar-profile environment.

### Environment
askar-profile

### Problem
After holder received credential from issuer, holder get empty results when getting credentials.

### Fix
Add `profile` parameter with `wallet.askar_profile` when scanning credentials


Thanks!

Signed-off-by: Ethan Sung <baegjae@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 04:37:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1509" class=".btn">#1509</a>
            </td>
            <td>
                <b>
                    Fix warnings when generating ReadTheDocs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: shaangill025 <gill.shaanjots@gmail.com>

- resolves #1506
- For duplicated object description, renamed references in `__init__.py`:
  - `vc.ld_proofs.crypto`, `vc.ld_proofs.purposes`, `vc.ld_proofs.suites` by adding a `_` when importing modules. Modified `vc.ld_proofs` to accomodate these changes
  -  `vc.vc_ld.models` by adding a `_` when importing modules. Modified `vc.vc_ld` accordingly
- For cross-reference warnings, adopted solution from [here](https://github.com/sphinx-doc/sphinx/issues/3866#issuecomment-768167824).
- Regarding`list not hashable` issue in `aries_cloudagent/protocols/issue_credential/v1_0/models/credential_exchange.py`, I think there was a minor bug/typo, we had `credential_request: [Mapping, IndyCredRequest] = None` instead of `credential_request: Union[Mapping, IndyCredRequest] = None`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 02:14:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1508" class=".btn">#1508</a>
            </td>
            <td>
                <b>
                    Fix error when connection request is received (askar, public invitation)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes error when connection request is received with public invitation under askar

### Environment
- connections/1.0 protocol
- public invitation
- askar

### Problem
Faber (invitation creator) encountered error below, when connection request was received.
```
2021-11-22 17:39:38,849 aries_cloudagent.core.dispatcher ERROR Handler error: Dispatcher.handle_message
Traceback (most recent call last):
  File "/Users/baegjae/src/aries-cloudagent-python/aries_cloudagent/core/dispatcher.py", line 197, in handle_message
    await handler(context, responder)
  File "/Users/baegjae/src/aries-cloudagent-python/aries_cloudagent/protocols/connections/v1_0/handlers/connection_request_handler.py", line 41, in handle
    await mgr.receive_request(
  File "/Users/baegjae/src/aries-cloudagent-python/aries_cloudagent/protocols/connections/v1_0/manager.py", line 592, in receive_request
    my_info = await wallet.create_local_did(DIDMethod.SOV, KeyType.ED25519)
  File "/Users/baegjae/src/aries-cloudagent-python/aries_cloudagent/wallet/askar.py", line 199, in create_local_did
    await self._session.handle.insert_key(
AttributeError: 'NoneType' object has no attribute 'insert_key'
```

`wallet` was inactive (=handle was None) when creating local did.

### Fix
This PR make `wallet` active to create local did.


Signed-off-by: Ethan Sung <baegjae@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 08:58:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1504" class=".btn">#1504</a>
            </td>
            <td>
                <b>
                    Remove Streetcred references
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 16:58:44 +0000 UTC
    </div>
</div>

