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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1364" class=".btn">#1364</a>
            </td>
            <td>
                <b>
                    fix: error not raised in predicate timestamp check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Quick fix for what appears to be a typo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 14:06:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1363" class=".btn">#1363</a>
            </td>
            <td>
                <b>
                    #1349 Added option to multitenant mode to handle multiple wallets inside the same subwallet with many Askar profiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This mode can be run by specifying `askar-profile` as the `wallet_type` in the CLI argument `--multitenancy-config`
Added `AskarProfileMultitenantManager` class which handles the new logic to get the wallet profile. The old logic was moved to `MultitenantManager`. The both extend `BaseMultitenantManager` where most of the previous code remained
The MultitenantManagerProvider chooses the right manager to use depending on the CLI argument
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 13:23:07 +0000 UTC
    </div>
</div>

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

