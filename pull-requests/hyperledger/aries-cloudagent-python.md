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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2305" class=".btn">#2305</a>
            </td>
            <td>
                <b>
                    Fix alice/faber demo execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the `--debug-webhooks` flag for all demo agents, as it is required to distinguish between credential offers and presentation requests for different credential types.

It also works around an issue with #2234 which causes the agents to exit with a RuntimeError due to the call to `loop.run_until_complete` within the logging configuration. I think a more complete fix might be to use a ContextVar to store the current DID identifier and set that when a tenant context is initialized, to avoid any async operations in the logger config.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 21:03:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2303" class=".btn">#2303</a>
            </td>
            <td>
                <b>
                    Cancel in-progress workflows when PR is updated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is meant to cancel in-progress unit tests and integration tests which are no longer valid, and only consuming resources.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 23:07:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2302" class=".btn">#2302</a>
            </td>
            <td>
                <b>
                    Update to indy-credx 1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 22:43:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2300" class=".btn">#2300</a>
            </td>
            <td>
                <b>
                    Feature: JWT Sign and Verify Admin Endpoints with DID Support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request introduces two new endpoints to the admin wallet API:

`POST /wallet/jwt/sign`: This endpoint allows for the creation of a JWS (JSON Web Signature) by providing a DID (Decentralized Identifier) or verification method along with a header and payload. The JWS is generated using the associated keys linked to the provided DID.

`POST /wallet/jwt/verify`: With this endpoint, you can verify a JWS by providing the JWS itself. The implementation includes a DID resolver, which leverages the JWS header to resolve a DID document. This document is then used to verify the signature of the provided JWS.

These new endpoints expand the functionality of our admin wallet API, empowering users to perform signing and verification operations conveniently. I have tested the code and ensured its compatibility with our existing system.

Signed-off-by: Adam Burdett <burdettadam@gmail.com>
Co-authored-by: Daniel Bluhm <daniel@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 18:39:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2299" class=".btn">#2299</a>
            </td>
            <td>
                <b>
                    Add build step for indy-base image in run_demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #2298 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 18:19:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2295" class=".btn">#2295</a>
            </td>
            <td>
                <b>
                    Allow any did to be public
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Having a universal resolver set in the configuration, I want to be able to create and receive invitations containing a public DID other than did:sov (Indy DID). In order to do that I must promote the DID to public after it has been created in the wallet.

This PR adds checks of the DID format to associate ledger operations to the did:sov only in the said operation, thus allowing any DID format to be set as public.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-11 12:42:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2294" class=".btn">#2294</a>
            </td>
            <td>
                <b>
                    Add Goal and Goal Code to OOB and DIDex Request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add support for `goal` and `goal_code` in API and messages for `out-of-band` and `didexchange`

Closes #1652
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 23:19:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2292" class=".btn">#2292</a>
            </td>
            <td>
                <b>
                    feat(anoncreds): Implement automated setup of revocation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements automated setup of revocation by introducing an `AnonCredsRevocationSetupManager` base class and `DefaultRevocationSetup` concrete class and adding the appropriate hooks to the artifact registration steps.

Overall, I'm very pleased with the simplicity of this setup manager as compared to our original mechanism. It works in more or less the same way, listening for events and triggering the next step in the flow; however, all the event listeners are defined in one place (rather than across 2 or 3 modules) and the event objects themselves have been formalized to make accessing the information in the event simpler. Additionally, encapsulation of the anoncreds interface is better than what we had previously so the event listeners themselves are fewer lines with significantly more straightforward logic.

I've left the door open for enabling plugins to implement their own `AnonCredsRevocationSetupManager` if there is ever a need to customize the setup behavior. I'm considering moving the `handle_full_registry` logic to this same component for the same reason -- giving plugin authors the ability to customize if needed -- but I'm not sure how likely it is anyone will actually need or want to do customizations.

This PR invalidates the following temporary endpoints we added for testing:

- `POST /anoncreds/revocation-registry-definition`
- `PUT /anoncreds/registry/{rev_reg_def_id}/tails-file`
- `PUT /anoncreds/registry/{rev_reg_def_id}/active`
- `POST /anoncreds/revocation-list`

I haven't removed these endpoints just yet in this PR though.

This PR adds `max_cred_num` to the expected options of the `POST /anoncreds/credential-definition` endpoint.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 15:03:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2291" class=".btn">#2291</a>
            </td>
            <td>
                <b>
                    fix: use python 3.9 in run_docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We overlooked one other instance of von-image getting used; this PR is a quick correction to the `Dockerfile.run` that gets used by the `run_docker` script.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 12:30:47 +0000 UTC
    </div>
</div>

