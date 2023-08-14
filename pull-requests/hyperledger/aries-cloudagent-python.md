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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2415" class=".btn">#2415</a>
            </td>
            <td>
                <b>
                    Remove Indy from tests run on PRs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed recently and captured in #2402, this PR removes Indy specific tests from PR test runs. This also adjusts other images and examples in the demo folder to use the non-indy variant of images.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 14:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2414" class=".btn">#2414</a>
            </td>
            <td>
                <b>
                    0.10.0-rc0
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
        Created At 2023-08-11 18:38:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2413" class=".btn">#2413</a>
            </td>
            <td>
                <b>
                    Fix: Ensure event/webhook is emitted for multi-use invitations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As a consequence of the fix in #2223, events/webhooks for new connections created responding to multi-use invitations were not being emitted. This happened because events are emitted, unless specified with the appropriate flag, only when the connection record being saved is new OR the state has changed.

Neither of those conditions is true for a multi-use invitation since the record is "cloned" and contextually set to state `request`  (see #2099). 

The fix ensures an event (and webhook) is always emitted when a new connection transitions to the `request` state.
Resolves #2406 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-11 02:38:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2412" class=".btn">#2412</a>
            </td>
            <td>
                <b>
                    Anoncreds API BDD Tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WIP - quick commit to see if tails server works on GH.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-11 02:21:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2409" class=".btn">#2409</a>
            </td>
            <td>
                <b>
                    feat: resolve connection targets and permit connecting via public DID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR builds on #2404 to adjust DID -> ConnectionTarget look up to use the DID Resolver interface and also to permit connecting via DID Exchange with public DIDs. This enables DIDComm over exclusively did:web and other methods (permits not rotating to a peer DID during the exchange) or just initializing a DID Exchange with a resolvable DID that supports DIDComm.

I believe this change is a significant improvement for consistently handling DIDs and DID Documents during connections as there is no longer a distinction between local/peer DIDs and public DIDs, at least in terms of determining how to look up the associated document.

This PR is currently in development. Once #2404 is in, I'll rebase this branch to clean up the history. There's a few more pieces I'm still working on as well:
- Unit tests. I've tested these changes manually and it's currently working as expected but I'll be a good citizen and make sure my additions are covered.
- Caching resolved DID Documents. This change relies on resolving DID Documents to determine connection targets. For exchanged (legacy) peer DIDs, this means it will look up the document in the wallet, which is more or less the same as it was before. However, if you're resolving public DIDs, we probably don't want to query a ledger every time we send a message, especially since DIDComm message exchanges tend to be burst-y. #2404 includes caching for legacy peer DIDs; however, I'm not certain whether caching should be handled at the method resolver layer or at the global resolver layer. I'll put some more thought into this.

cc @swcurran @Jsyro I'll elaborate how I think this should affect the Peer DID work further in #2249 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 14:59:23 +0000 UTC
    </div>
</div>

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

