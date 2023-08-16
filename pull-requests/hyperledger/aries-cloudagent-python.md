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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2423" class=".btn">#2423</a>
            </td>
            <td>
                <b>
                    the anoncreds proof presentation with schema restriction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                missed this file... 🤦 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 22:04:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2421" class=".btn">#2421</a>
            </td>
            <td>
                <b>
                    Issue #2250 Nightly publish workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This issue resolves #2250

Here I have created a GitHub workflow that will execute the tests just as they are handled in `nightly-tests.yml` excluding the indy tests as mentioned in this comment.

https://github.com/hyperledger/aries-cloudagent-python/issues/2250#issuecomment-1674918887

The workflow acts as follows
```python
run nightly tests
If (tests are successful):
   build a nightly release
   publish this release with the `nightly` tag
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 15:47:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2420" class=".btn">#2420</a>
            </td>
            <td>
                <b>
                    Issue #2419 InvalidClientTaaAcceptanceError time too precise error if container timezone is not UTC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds timezone.utc to datetime.combine to ensure time will be midnight in UTC regardless of the default timezone
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 23:16:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2418" class=".btn">#2418</a>
            </td>
            <td>
                <b>
                    Enable Snyk scanning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                addresses #2087 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 20:23:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2416" class=".btn">#2416</a>
            </td>
            <td>
                <b>
                    feat: Proof Negotiation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a rebased version of #2033. Thank you for your contributions, @Przytua!

I think these changes are likely to be better suited to a new endpoint (i.e. `POST /present-proof/{pres_ex_id}/counter-request` or something) rather than changing the behavior of `POST /present-proof/{pres_ex_id}/request`. I'll open this as a draft for now and look at making these changes when I can.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 19:01:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2415" class=".btn">#2415</a>
            </td>
            <td>
                <b>
                    Remove Indy tests from workflows
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
                Add BDD tests for issue v2 and proof presentation v2.
The tests include create schema, create cred def and revocation through the new `/anoncreds` API.

Note that I encountered some weirdness running the tests in the devcontainer... some messages didn't appear to be fully fleshed out (see comments about "by_format"). Running using the `run_bdd` script was fine.

Also, on proof presentation, I could not get it working using restriction with "schema_name" and "schema_version" like other presentations. I used restrictions by `cred_def_id` to pass the tests.  Not sure if that is something that needs to be looked at further as it would impact migrations to `anoncreds` if current presentation requests don't work.


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

