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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1359" class=".btn">#1359</a>
            </td>
            <td>
                <b>
                    Updates to the Read The Docs for 0.7.0/1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates various files necessary to generate the Read The Docs files about ACA-Py.  Should have been done before the tagging of 0.7.0 -- my miss.

Mostly complete, with two classes of warnings in the generation process remaining as follows:

1. One instance of this:

```bash
WARNING: error while formatting arguments for aries_cloudagent.protocols.issue_credential.v1_0.models.credential_exchange.V10CredentialExchange: unhashable type: 'list'
```

2. Nine instances with the same symptom referencing `__all__`, here are two:

```
WARNING: __all__ should be a list of strings, not [typing.Callable[[str, dict], dict], <class 'aries_cloudagent.vc.ld_proofs.document_loader.DocumentLoader'>] (in module aries_cloudagent.vc.ld_proofs.document_loader) -- ignoring __all__
WARNING: __all__ should be a list of strings, not [<class 'aries_cloudagent.vc.ld_proofs.crypto.KeyPair.KeyPair'>, <class 'aries_cloudagent.vc.ld_proofs.crypto.WalletKeyPair.WalletKeyPair'>] (in module aries_cloudagent.vc.ld_proofs.crypto) -- ignoring __all__

```

If anyone knows how to address that, please do.

To reproduce the errors on this branch, follow the instructions in the `readme.md` file in the \docs folder (install sphinx, run the build command).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 04:17:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1356" class=".btn">#1356</a>
            </td>
            <td>
                <b>
                    fix: problem report handler for connection specific problems
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Appears to be an error leftover from when the problem report message definition was relocated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 19:26:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1352" class=".btn">#1352</a>
            </td>
            <td>
                <b>
                    fix: deepcopy attach decorator data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @Moopli had an interop issue between AFGO and ACA-Py. It came down to ACA-Py modifying the json returned from an attachment decorator which would cause issues later on because the object was missing some expected properties. (see more info below)

To prevent such mistakes in the future it is now fixed by making a deep copy both when setting and retrieving json from an attachment decorator. I'm not 100% what the impact of this is on performance, and whether json.dumps and json.loads may be faster.

We could also fix it by making a copy in the json ld handler, but this won't fix the issue all together. @andrewwhitehead I'm interested to hear which approach you'd take.

> TimoGlastra I found the bug
from here:
https://github.com/hyperledger/aries-cloudagent-python/blob/main/aries_cloudagent/protocols/issue_credential/v2_0/manager.py#L571
we end up calling ld_proof/handler LDProofCredFormatHandler.receive_credential, and when it gets here:
https://github.com/hyperledger/aries-cloudagent-python/blob/main/aries_cloudagent/protocols/issue_credential/v2_0/formats/ld_proof/handler.py#L493
it modifies the original attachment in the message, removing the proof member from the credential. So when the ld proof handler returns, V20CredManager stores the damaged message, causing the later error on deserialization.
The issue is, AttachDecorator returns json attachments by reference: https://github.com/hyperledger/aries-cloudagent-python/blob/main/aries_cloudagent/messaging/decorators/attach_decorator.py#L560
To fix this issue alone, LDProofCredFormatHandler.receive_credential could simply build a shallow copy of cred_dict
but I imagine that where one bug appears, others lurk in silence - is AttachDecorator` supposed to provide a mutable reference? Or should it return a deep copy of the dict?
the workaround I'm doing right now is to make the issued credential a b64 attachment instead
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 20:33:25 +0000 UTC
    </div>
</div>

