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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1605" class=".btn">#1605</a>
            </td>
            <td>
                <b>
                    Replace blank credential/presentation exchange states with abandoned state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to #1588 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 19:33:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1604" class=".btn">#1604</a>
            </td>
            <td>
                <b>
                    WIP: Inbound and Outbound Persistent Message Queues, Redis and Kafka 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1513 
![image](https://user-images.githubusercontent.com/9292265/150176209-66f2954c-2f89-47dc-916b-57ae8d6dbdbf.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 15:33:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1603" class=".btn">#1603</a>
            </td>
            <td>
                <b>
                    Update aries-askar patch version to at least 0.2.4 as 0.2.3 does not include backward compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Issue

- When signing the proof presentation or credential using BLS key created before the aries-askar update the process fails with:


```
File "/aries-cloudagent-python/aries_cloudagent/wallet/askar.py", line 592, in sign_message
key = keypair.key
File "/usr/local/lib/python3.6/site-packages/cached_property.py", line 36, in __get__
value = obj.__dict__[self.func.__name__] = self.func(obj)
File "/usr/local/lib/python3.6/site-packages/aries_askar/store.py", line 147, in key
return Key(self._list.load_key(self._pos))
File "/usr/local/lib/python3.6/site-packages/aries_askar/bindings.py", line 210, in load_key
byref(handle),
File "/usr/local/lib/python3.6/site-packages/aries_askar/bindings.py", line 531, in do_call
raise get_current_error(True)
aries_askar.error.AskarError: Unsupported JWK for key import
The above exception was the direct cause of the following exception:
Traceback (most recent call last):
File "/usr/local/lib/python3.6/site-packages/ddtrace/contrib/aiohttp/middlewares.py", line 61, in attach_context
response = await handler(request)
File "/aries-cloudagent-python/aries_cloudagent/admin/server.py", line 163, in ready_middleware
return await handler(request)
File "/aries-cloudagent-python/aries_cloudagent/admin/server.py", line 200, in debug_middleware
return await handler(request)
File "/usr/local/lib/python3.6/site-packages/aiohttp_apispec/middlewares.py", line 45, in validation_middleware
return await handler(request)
File "/aries-cloudagent-python/aries_cloudagent/admin/server.py", line 339, in check_multitenant_authorization
return await handler(request)
File "/aries-cloudagent-python/aries_cloudagent/admin/server.py", line 383, in setup_context
return await task
File "/aries-cloudagent-python/aries_cloudagent/protocols/present_proof/v2_0/routes.py", line 1072, in present_proof_send_presentation
comment=comment,
File "/aries-cloudagent-python/aries_cloudagent/protocols/present_proof/v2_0/manager.py", line 264, in create_pres
request_data,
File "/aries-cloudagent-python/aries_cloudagent/protocols/present_proof/v2_0/formats/dif/handler.py", line 371, in create_pres
records_filter=limit_record_ids,
File "/aries-cloudagent-python/aries_cloudagent/protocols/present_proof/dif/pres_exch_handler.py", line 1290, in create_vp
document_loader=document_loader,
File "/aries-cloudagent-python/aries_cloudagent/vc/vc_ld/prove.py", line 101, in sign_presentation
document_loader=document_loader,
File "/aries-cloudagent-python/aries_cloudagent/vc/ld_proofs/ld_proofs.py", line 41, in sign
document_loader=document_loader,
File "/aries-cloudagent-python/aries_cloudagent/vc/ld_proofs/proof_set.py", line 53, in add
document=input, purpose=purpose, document_loader=document_loader
File "/aries-cloudagent-python/aries_cloudagent/vc/ld_proofs/suites/bbs_bls_signature_2020.py", line 82, in create_proof
proof = await self.sign(verify_data=verify_data, proof=proof)
File "/aries-cloudagent-python/aries_cloudagent/vc/ld_proofs/suites/bbs_bls_signature_2020.py", line 181, in sign
signature = await self.key_pair.sign(verify_data)
File "/aries-cloudagent-python/aries_cloudagent/vc/ld_proofs/crypto/wallet_key_pair.py", line 38, in sign
from_verkey=self.public_key_base58,
File "/aries-cloudagent-python/aries_cloudagent/wallet/askar.py", line 604, in sign_message
raise WalletError("Exception when signing message") from err
aries_cloudagent.wallet.error.WalletError: Exception when signing message
```

- Temporary fix is to limit dependency to 0.2.2

- The renaming done in https://github.com/hyperledger/aries-askar/pull/31/files#diff-9a004bebad212a7cc70871d55577ebd32f8dbff770e029d927abc4535435cf3cR539  seems to be a breaking change.

@andrewwhitehead Can you please take a look and advise on a proper fix?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 15:10:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1601" class=".btn">#1601</a>
            </td>
            <td>
                <b>
                    DID updates for endorser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Adds endorser support to the ledger register_nym function, allowing Authors to self-register a public DID.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 00:08:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1599" class=".btn">#1599</a>
            </td>
            <td>
                <b>
                    did-exchange implicit request pthid update & invitation key verification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
resolve #1595 
resolve #1594 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-13 23:23:44 +0000 UTC
    </div>
</div>

