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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2404" class=".btn">#2404</a>
            </td>
            <td>
                <b>
                    feat: add legacy peer did resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds support for resolving legacy peer DIDs to DID Documents previously stored in our wallet.

This is one part of some additional changes I have in mind; using these changes, I'd like to make "resolving" connection targets for a DID consistent regardless of whether the DID we're resolving is did:web, did:indy, did:sov, unqualified local did, did:peer, etc. I'm hopeful those changes will also help ease the transition to proper peer DIDs. I'm still fleshing out those changes but I think this resolver is useful regardless of the outcome.

As noted in the docstrings of the methods in the resolver, due to the nature of ACA-Py's use of did:sov and unqualified DIDs for both public (posted to a ledger) and pairwise/peer DIDs, this resolver requires a bit of trial and error. If the DID has a doc associated with it in the wallet, it will report that it supports resolving the DID. The cache is employed to help make this check slightly more efficient but there's still some open questions. For instance, how long should the cache be considered valid?

As implemented, this resolver will only return the DID Documents we've received through the Connections or DID Exchange protocols. In other words, we can only resolve the DID of the remote party, or "their DID." We could also store the docs for our own DIDs, making them resolvable as well. I'm not sure if this is valuable or not yet.

For Indy "style" DIDs that are created outside of the context of a connection, such as Public DIDs, there is no DID Document associated with it stored in our wallet. This means that this resolver will not be selected and the document for the DID will be resolved by the `IndyDIDResolver`, as usual.

In the interest of that consistent connection target goal I mentioned above, I currently have this resolver configured to transform documents retrieved from our wallet to be better aligned with updates to DIDComm/DID Document conventions.

Resolves #2161. I think. lol
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-09 02:35:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2401" class=".btn">#2401</a>
            </td>
            <td>
                <b>
                    Anoncreds BDD test preparation.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Relates to #2297.

This is step one to onboard `anoncreds-rs`. 

Changes to ledger base classes has "broken" schemas and cred defs. This is expected as we are transition. This PR merely allows us to run `BDD` tests, `pytest`, `Flake8` and `black` so we can commit and merge future PRs.

BDD tests that are failing due to anoncreds restructuring of Base ledger are now labelled/tagged: `@GHA-Anoncreds-break`. Fix and reintroduce these tests as needed.

Flake8 class documentation is a placeholder, these have: `TODO: update this docstring - Anoncreds-break.` and should be updated with useful documentation.

Pytests that are broken have been skipped with: `@pytest.mark.skip(reason="Anoncreds-break")`.

Please note that I have added in the `devcontainer` from `main`.

BDD Tests Run:

```
LEDGER_URL=http://test.bcovrin.vonx.io PUBLIC_TAILS_URL=https://tails-test.vonx.io LOG_LEVEL=warning NO_TTY=1 ./run_bdd -t @GHA```

BDD Tests Results:

```
2 features passed, 0 failed, 3 skipped
7 scenarios passed, 0 failed, 57 skipped
37 steps passed, 0 failed, 703 skipped, 0 undefined
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-07 18:58:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2399" class=".btn">#2399</a>
            </td>
            <td>
                <b>
                    Upgrade pre-commit and flake8 dependencies; fix flake8 warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Edit: flake8 must remain pinned to v4.0 as pytest-flake8 is unmaintained and doesn't support flake8 > 5.0 (latest = 6.1)
I propose migrating to [ruff](https://beta.ruff.rs/docs/) and [pytest-ruff](https://github.com/businho/pytest-ruff). Created issue: https://github.com/hyperledger/aries-cloudagent-python/issues/2400

___

Upgrades `.pre-commit-config.yaml` to use latest versions for pre-commit-hook, black, and flake8.
This fixes pre-commit not being in sync with black/flake8 enforcement in the github actions.

Additionally we upgrade flake8, flake8-docstrings, and pydocstyle to latest. 

Includes fixes for all flake8 warnings in ./aries_cloudagent, because if PR tests enforces flake8, then the existing code should abide by it too :-)

The remaining flake8 warnings are primarily for missing docstrings in ./demo
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-06 09:34:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2398" class=".btn">#2398</a>
            </td>
            <td>
                <b>
                    Chore: fix marshmallow warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #2342

I used the [acapy-marshmallow-upgrade](https://github.com/dbluhm/acapy-marshmallow-upgrade) tool created by @dbluhm (as described here: https://github.com/hyperledger/aries-cloudagent-python/pull/1854#issuecomment-1189381980), which iterates over usages of marshmallow fields, to wrap deprecated arguments in a metadata dictionary.

The only hairy part to this task was the schemas defined in `aries_cloudagent/messaging/valid.py`:
```py
INT_EPOCH = {"validate": IntEpoch(), "example": IntEpoch.EXAMPLE}
WHOLE_NUM = {"validate": WholeNumber(), "example": WholeNumber.EXAMPLE}
# etc ...
```
These definitions were used in marshmallow fields by calling e.g. `fields.Int(..., **INT_EPOCH)`, which would be missed by the upgrade tool. Also, validate is a supported argument, while example should be moved to metadata.

To account for this, I refactored the schema specifications (using regex):
```py
INT_EPOCH_VALIDATE = IntEpoch()
INT_EPOCH_EXAMPLE = IntEpoch.EXAMPLE

WHOLE_NUM_VALIDATE = WholeNumber()
WHOLE_NUM_EXAMPLE = WholeNumber.EXAMPLE
# etc ...
```

I then updated the imports, and replaced usages of `**INT_EPOCH`, for example, to `validate=INT_EPOCH_VALIDATE, example=INT_EPOCH_EXAMPLE`. Then could I run the marshmallow-upgrade tool created by dbluhm to correctly wrap examples in the metadata.

Additionally: upgrade marshmallow to latest (3.20)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-05 10:42:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2395" class=".btn">#2395</a>
            </td>
            <td>
                <b>
                    Multitenant check endorser_info before saving
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While testing PR #2339 I was using an instance without an endorser and encountered an error while saving the new write ledger: `UnboundLocalError: local variable 'endorser_alias' referenced before assignment`.

This checks to see if we have endorser information before we try to persist it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 18:50:09 +0000 UTC
    </div>
</div>

