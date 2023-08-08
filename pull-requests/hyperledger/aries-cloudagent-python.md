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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2394" class=".btn">#2394</a>
            </td>
            <td>
                <b>
                    feat: add DID Exchange specific problem reports and reject endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes problem reports sent during the DID Exchange protocol have the DID Exchange protocol adopted problem report rather than the generic problem report. This is defined in RFC 23 but has not been implemented by ACA-Py to this point. In other words, this is a correction to bring ACA-Py more in line with the RFC. These problem reports were automatically sent if there was an issue in processing the DID Exchange messages.

In addition to the above changes, this PR also introduces a `POST /didexchange/{conn-id}/reject` endpoint, enabling the controller to explicitly reject an OOB invitation that specifies DID Exchange as the handshake protocol or a DID Exchange request. Rejecting a response is not supported; don't send a request if you're going to reject the response. This will send a problem report to the originator of the invitation/request and will mark the (local) connection record as abandoned. It won't delete the record though (maybe it should)?

This at least partially supersedes #2350, covering the rejection of invitations to exchange DIDs. However, it does not introduce automatic handling of timeouts for invitations, as was discussed in the comments.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 13:27:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2393" class=".btn">#2393</a>
            </td>
            <td>
                <b>
                    fix: outbound send status missing on path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This corrects a flow through the `queue_outbound` method that could result in no `OutboundSendStatus` being returned. The method is strictly expected to return a status so this could cause less than graceful errors in some circumstances.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 11:52:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2392" class=".btn">#2392</a>
            </td>
            <td>
                <b>
                    fix: additional tweaks for did:web and other methods as public DIDs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adjusts the request schema for the set public DID endpoint to permit `GENERIC_DID`s. It seems that the work to support a generic DID in this endpoint was already done and just the request schema was missed by mistake (or perhaps it's a merge artifact :man_shrugging:).

Additionally, this PR adjusts the behavior of DID Exchange requests so that if we're using a public DID, no DID Doc attachment is included in the request. This enables us to form connections using a did:web or other DID that is resolvable without worrying about ACA-Py's DID Doc creation process not being quite up to snuff on multi-method support.

And some minor type hint corrections.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-01 19:00:14 +0000 UTC
    </div>
</div>

