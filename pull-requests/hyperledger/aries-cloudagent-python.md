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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2827" class=".btn">#2827</a>
            </td>
            <td>
                <b>
                    Integration tests - Add retry to did registration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Seeing if adding a did registry retry helps the intermittently failing tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-06 18:41:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2825" class=".btn">#2825</a>
            </td>
            <td>
                <b>
                    0.12.0rc2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes some cleanup of the docs for static site generation -- mostly in MD files, but also in the GHA for generating the docs -- links to docs that are different between the repo and the generated docs.

Still no breaking changes to note.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 23:07:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2824" class=".btn">#2824</a>
            </td>
            <td>
                <b>
                    patch for #2781: User Agent header in doc loader
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                a patch for #2781 (see issue description). Longer term acapy may consider making a User Agent header globally for all requests, and perhaps configurable. however this one gets us by
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 21:52:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2823" class=".btn">#2823</a>
            </td>
            <td>
                <b>
                    Support connection re-use for did:peer:2/4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See issue https://github.com/hyperledger/aries-cloudagent-python/issues/2703

This PR is WIP, still need to do a bunch of testing.

- adds additional meta-data to the wallet DID, to flag a did:peer for re-using in invitations
    - is this acceptable?  ***
- add the DID meta-data to the admin API `GET /wallet/did` response
    - is this acceptable?  it's necessary to find an existing re-usable invitation DID ...  ***
- add a flag to the OOB create invitation to request a unique did (default is to re-use the invitation DID in the wallet)
- reuse works for did:peer:2 and did:peer:4, and also public DID
    - should this be generic?  and how to determine if the DID can be used for connection reuse?  should it work for ALL DID methods?  ***
- added separate flags to the demo for:
	- `--public-did-connections` - use the inviter's public DID in invitations, and allow use of implicit invitations
	- `--reuse-connections` - support connection re-use (invitee will reuse an existing connection if it uses the same DID as in the new invitation)
	- `--multi-use-invitations` - inviter will issue multi-use invitations
	- note that the `--reuse-connections` flag needs to be enabled in both Faber and Alice for the demo to enable connection reuse

*** see questions above

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 18:38:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2822" class=".btn">#2822</a>
            </td>
            <td>
                <b>
                    Anoncreds - support for anoncreds and askar wallets concurrently
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implements https://github.com/hyperledger/aries-cloudagent-python/issues/2807.

1. Enables schema, cred_def and revocation endpoints for both askar and askar-anoncreds in multitenant mode. All anoncreds endpoints are prefixed with `/anoncreds/`. For some api marshmallow schema objects they were the same name as the existing  objects which displayed a warning. I simply appended Anoncreds to the end of these objects that had conflicts.
3. Returns 403 errors when using the wrong endpoints with message. I thought about trying to do something fancier like a middleware, but decided because it was only a small subset that it would be easier to just add a method to the top of the endpoints. In anoncreds some of the endpoints already had a profile type check and through a ValueError. I did handle this, but for consistency and to prevent unrelated errors I still added the profile check method to the top of the method.
4. Prevent subwallets from being created that are a different type then the base wallet. For example, in the case of having the base wallet askar and trying to create a askar-anoncreds wallet it will throw a 403 and have a message. If the wallet type is empty is defaults to the base wallet.
5. Prevents wallets from being started as an askar wallet and then trying to change the config to askar-anoncreds by using a similar flow as versioning. If the `wallet-type` record is empty and there is a version record (existing wallet) it will assume the wallet is askar. I'm still unsure if anything needs to happen with `indy` wallets. I'm having trouble installing the library to test.
6. Updates integration tests and runs a few of the tests that touch most of the effected endpoints in multitenancy mode.
7. Updates the faber agent in the demos.

Going to leave in draft state and target next release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 00:10:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2821" class=".btn">#2821</a>
            </td>
            <td>
                <b>
                    Send revocation list instead of rev_list object - Anoncreds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes anoncreds specific problem on initial rev_list. Was sending the rev_list object to the event handler instead of the actual list.

Added a log message to v1 handler for after the message has been sent.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 18:56:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2820" class=".btn">#2820</a>
            </td>
            <td>
                <b>
                    FIX: GHA update for doc publishing, fix doc file that was blanked
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Next try (if needed) will get into the regex...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 22:15:25 +0000 UTC
    </div>
</div>

