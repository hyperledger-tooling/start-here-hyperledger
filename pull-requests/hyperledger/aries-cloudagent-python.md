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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2290" class=".btn">#2290</a>
            </td>
            <td>
                <b>
                    1.0.0-rc3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR to enable creating a 1.0.0-rc3 release that matches ACA-Py Release 0.8.2.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 21:02:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2288" class=".btn">#2288</a>
            </td>
            <td>
                <b>
                    Fix routing in set public did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Having a multitenancy mode and a base wallet mediator, when a DID was being promoted to public the base wallet mediator was not taken into consideration - the returned mediation record was always None. As a result, the agent's endpoint is written to ledger instead of the mediator's.

This PR fixes this issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 09:50:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2287" class=".btn">#2287</a>
            </td>
            <td>
                <b>
                    Webhook over websocket clarification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Supersedes #2220. Thank you for your contributions @miroslav-inc!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-05 13:51:22 +0000 UTC
    </div>
</div>

