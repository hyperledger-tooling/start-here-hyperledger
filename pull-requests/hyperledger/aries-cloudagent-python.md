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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2356" class=".btn">#2356</a>
            </td>
            <td>
                <b>
                    :rocket: Performance Boost: Replace json with orjson through JsonUtil class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The [orjson](https://github.com/ijl/orjson) library provides superior performance over the built-in json module. Please see their readme for an overview of features and performance/runtime comparisons.

One note is: `orjson.dumps` serializes to `bytes`, instead of `str`, so it's not a drop in replacement.
Edit: it also omits whitespace between keys and values. i.e. json.dumps: `{"k": [1, 2, 3]}`. orjson.dumps:  `{"k":[1,2,3]}`

There are 449 usages of `json.dumps` throughout the codebase. To refactor, I would just want to regex replace all of those with `orjson.dumps`, but then it would require appending `.decode()` as well (for bytes -> string).

That inspired me to create a JsonUtil class in `utils.json.py`. So, I could replace all instances of `json.loads` and `json.dumps` with `JsonUtil.*`.

This also has the benefit of providing an abstraction layer to simplify future transitions between different JSON libraries.

Note: I had to replace `import json` with `from aries_cloudagent.utils.json import JsonUtils`. Re-added `import json` where needed. However, that means the import organisation is no longer consistent, because json is a top-level import, and the utils import shouldn't be. Nitpick, bit I would want to do a import sort across all files to fix this ...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 17:40:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2355" class=".btn">#2355</a>
            </td>
            <td>
                <b>
                    Correct the response type in `send_rev_reg_def`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Simple fix: the `send_rev_reg_def` method can return a `rev_reg: IssuerRevRegRecord`, which doesn't line up with the expected schema (`TxnOrRevRegResultSchema`).

TLDR: 
- the OpenAPI spec says the response is a `TxnOrRevRegResultSchema`, 
- but it's actually a `Union[RevRegResult, TxnOrRevRegResult]`.

As the name suggests, the `RevRegResult` should be wrapped in a `TxnOrRevRegResult`, which this PR fixes.

Initially typed out an issue, so just to show my working:
___
In the definition for the `send_rev_reg_def` method (in [`/aries_cloudagent/revocation/routes.py`](https://github.com/hyperledger/aries-cloudagent-python/blob/8b6c87fba2a6dc6cce4ced92d4db554fb4cad37a/aries_cloudagent/revocation/routes.py#L1019)), the response schema is indicated to be a `TxnOrRevRegResultSchema`:
```py
@response_schema(TxnOrRevRegResultSchema(), 200, description="")
async def send_rev_reg_def(request: web.BaseRequest):
```
which has the definition:
```py
class TxnOrRevRegResultSchema(OpenAPISchema):
    """Result schema for credential definition send request."""

    sent = fields.Nested(
        RevRegResultSchema(),
        required=False,
        definition="Content sent",
    )
    txn = fields.Nested(
        TransactionRecordSchema(),
        required=False,
        description="Revocation registry definition transaction to endorse",
    )
```

In the [`aries-cloudcontroller-python`](https://github.com/didx-xyz/aries-cloudcontroller-python) project, we have to manually alter the model, generated from the OpenAPI spec, to correct that the response can actually be a `Union[RevRegResult, TxnOrRevRegResult]`, because that's what the server gives.

So, something is wrong with the implementation. Let's inspect [the code](https://github.com/hyperledger/aries-cloudagent-python/blob/8b6c87fba2a6dc6cce4ced92d4db554fb4cad37a/aries_cloudagent/revocation/routes.py#L1019):
```py
@response_schema(TxnOrRevRegResultSchema(), 200, description="")
async def send_rev_reg_def(request: web.BaseRequest):
    ...
    if not create_transaction_for_endorser:
        return web.json_response({"result": rev_reg.serialize()})

    else:
        ...
        return web.json_response({"txn": transaction.serialize()})
```

There are two return statements, providing either `rev_reg: IssuerRevRegRecord`, or `transaction: TransactionRecord`.

The problem seems to be the key "result" that's being used in the rev_reg response, which should presumably be "sent", in order to correctly map to the key in the `TxnOrRevRegResultSchema`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 10:58:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2354" class=".btn">#2354</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump certifi from 2023.5.7 to 2023.7.22 in /demo/playground/scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [certifi](https://github.com/certifi/python-certifi) from 2023.5.7 to 2023.7.22.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/8fb96ed81f71e7097ed11bc4d9b19afd7ea5c909"><code>8fb96ed</code></a> 2023.07.22</li>
<li><a href="https://github.com/certifi/python-certifi/commit/afe77220e0eaa722593fc5d294213ff5275d1b40"><code>afe7722</code></a> Bump actions/setup-python from 4.6.1 to 4.7.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/230">#230</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/2038739ad56abec7aaddfa90ad2ce6b3ed7f5c7b"><code>2038739</code></a> Bump dessant/lock-threads from 3.0.0 to 4.0.1 (<a href="https://redirect.github.com/certifi/python-certifi/issues/229">#229</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/44df761f4c09d19f32b3cc09208a739043a5e25b"><code>44df761</code></a> Hash pin Actions and enable dependabot (<a href="https://redirect.github.com/certifi/python-certifi/issues/228">#228</a>)</li>
<li>See full diff in <a href="https://github.com/certifi/python-certifi/compare/2023.05.07...2023.07.22">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2023.5.7&new-version=2023.7.22)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 23:10:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2353" class=".btn">#2353</a>
            </td>
            <td>
                <b>
                    Accept did:peer:2 and optionally send. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Backwards compatible with older agents and existing unqualified dids.

Added flows that accept and send `did:peer:2` within DIDExchange protocol, however sends by default. 

Custom DIDDoc class from acapy exists, however upon deserialization will converted into a pydid DIDDocument instance. the existing Custom DIDDoc class is not compliant with the CONTEXT attribute it provides. 

Remaining work: 

- [ ] Clean up debugging and WIP shrapnel. 
- [ ] promote pydid and peer-did-python alpha changes to actual releases.
- [ ] Ensure it will work with upgrading acapy when the agent already has an existing connection
- [ ] Ability to promote/convert existing connections' did documents to did:peer:3 (see https://github.com/hyperledger/aries-cloudagent-python/issues/2345)
- [ ] Tests


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 23:05:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2352" class=".btn">#2352</a>
            </td>
            <td>
                <b>
                    Extend `--preserve-exchange-records` to include Presentation Exchange.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add `auto_remove` flags to appropriate APIs for override of default behaviour.

Verifiers/Provers can override default behaviour in `send-request` (both free presentation and bound presentation), `send-presentation`, `send-proposal`.

Note: added `auto_remove` to issue credentials (1 and 2) `send-request`, allowing holders to override the default behaviour.


Closes #2126 
Closes #2206 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 19:26:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2350" class=".btn">#2350</a>
            </td>
            <td>
                <b>
                    Oob problem report
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Supersedes #2150. Closes #2101. I am volunteering to help get this change in; looks like things are nearly there, just need to fix some issues with tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 17:00:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2348" class=".btn">#2348</a>
            </td>
            <td>
                <b>
                    Extract getting verification key for proof signing into VerificationKeyStrategy class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following the logic in PR [2235](https://github.com/hyperledger/aries-cloudagent-python/pull/2235) it is also beneficial to have the strategy for getting verification key itself overridable by plugins.

Such a use case would be to use the universal resolver to get a DID Document and fetch a verkey identified by the key ID. Then search the wallet by the verkey to obtain DIDInfo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 12:08:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2344" class=".btn">#2344</a>
            </td>
            <td>
                <b>
                    0.9.0
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
        Created At 2023-07-24 20:03:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2343" class=".btn">#2343</a>
            </td>
            <td>
                <b>
                    Add more context to the ACA-Py Revocation handling documentation
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
        Created At 2023-07-24 18:12:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2341" class=".btn">#2341</a>
            </td>
            <td>
                <b>
                    fix: ensure request matches offer, if sent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change implements checking that ld proof credential requests match their corresponding offer, if an offer was sent.

If using the `--auto-*` flags for issuance, it was possible for the receiver of the credential offer to change values in the request and ACA-Py would accept this and issue based off of the request values. The `--auto-*` flags are debug flags and should not be used in production which would mean that a controller should have been able to catch this discrepancy. However, it is still expedient for ACA-Py to check that the offer and request match to avoid this slipping past the controller as well.

There is a side affect of this check. We were permitting late binding of the credential subject ID to the holder in the request. Meaning, on request, the holder will automatically (when using auto flags) insert a DID key as the credential subject ID to ensure the holder can actually present proof of possession later. These changes modify this behavior such that it only applies iff the credential subject id is not set already (e.g. in the credential offer). This enables the issuer to bind the credential to a DID other than the holder's pairwise DID if an alternate is known to the issuer. If the issuer wants to permit late binding by the holder still, the credential subject ID should be omitted in the offer.

So, to summarize, the two modifications implemented here:
- Ensure the request doesn't change the credential unless the offer explicitly omits a credential subject ID
- Only override with holder did if the credential subject ID is omitted
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 14:32:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2340" class=".btn">#2340</a>
            </td>
            <td>
                <b>
                    Document the Indy SDK to Askar Migration process
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
        Created At 2023-07-21 23:08:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2339" class=".btn">#2339</a>
            </td>
            <td>
                <b>
                    Feat: Support Selectable Write Ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2168 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 15:57:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2338" class=".btn">#2338</a>
            </td>
            <td>
                <b>
                    0.9.0-rc0
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
        Created At 2023-07-21 13:53:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2336" class=".btn">#2336</a>
            </td>
            <td>
                <b>
                    ⬆️ upgrade `requests` to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `requests` dependency for ACA-py is currently using version `2.25.1` (Dec 2020), and has seen numerous improvements since then ito vulnerability fixes, speed optimizations, and support for python 3.10+

See changelogs here: https://github.com/psf/requests/releases
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 09:08:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2335" class=".btn">#2335</a>
            </td>
            <td>
                <b>
                    ⬆️ upgrade `pyjwt` to latest; introduce leeway to `jwt.decode`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Latest release (2.8) introduces support for python 3.10+

Release notes: https://github.com/jpadilla/pyjwt/releases

Note: `jwt.decode` can fail spuriously due to breaking changes introduced in https://github.com/jpadilla/pyjwt/pull/797, where an exception is raised if the 'issued at' time of the JWT is in the future when decoding, with default 0 leeway. This means that a miniscule mismatch in clock synchronization, between generation and decoding of JWT, can now cause a failure when decoding. This arose in the integration tests, and is resolved with a leeway of 1 second.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 09:02:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2334" class=".btn">#2334</a>
            </td>
            <td>
                <b>
                    ⬆️ upgrade `packaging` to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `packaging` dependency is pinned to version 20. This is incompatible with the latest release of the `black` formatter:
```
black 23.7.0 requires packaging>=22.0, but you have packaging 20.9 which is incompatible.
```

There doesn't seem to be any breaking changes in the new packaging release, so this PR bumps the dependency to latest
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 08:32:27 +0000 UTC
    </div>
</div>

