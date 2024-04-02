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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2862" class=".btn">#2862</a>
            </td>
            <td>
                <b>
                    refactor: introduce use_did and use_did_method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This implements #2857. With one modification: rather than having a single parameter `use_did`, I found that the processing became significantly simpler by having a `use_did` and `use_did_method` parameter. Hopefully that's an acceptable trade off.

WIP: Currently, just the updates to the did exchange routes have been made. Working through the OOB route updates now. Wanted to open early for feedback.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 19:55:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2861" class=".btn">#2861</a>
            </td>
            <td>
                <b>
                    feat: Integrate AnonCreds with W3C VCDI Format Support in ACA-Py
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Summary
Pull request introduces comprehensive support for AnonCreds within the W3C VCDI formats. The changes include the addition of new models, methods, and protocols that enable the Aries Cloud Agent Python to issue, hold, and verify credentials in alignment with W3C's VCDI standards.

### Changes Overview

- AnonCreds Integration: Updated the anoncreds module to handle VCDI-compliant credential offers, requests, and credentials.
- Indy Models: Adapted indy/models to map onto VCDI credential.
- Issue Credential Protocol v2.0: Incorporated VCDI support into the existing issue_credential protocol
- VCDI Credential Format Handling: Introduced a new vc_di module within formats to handle the specificities of the VCDI credential format.
- Updated alice/faber demo: Introduced handling of multiple cred demo with cred-type argument

### Detailed Changes

- Added handler.py in protocols/issue_credential/v2_0/formats/vc_di to manage VCDI credential operations.
- Created test_handler.py in the same directory to ensure robustness and reliability through comprehensive testing.
- Introduced vc_di.py within models/detail for detailed VCDI model definitions.
- Updated test_routes.py to test the integration of VCDI routes within the agent's service layer.
- Revised routes.py to handle API endpoints related to VCDI credential operations.
- Updated faber.py
- Update alice.py
- Updated agent_container.py
- Updated performance.py


### Additional Notes
Link to the detailed documentation and specifications: [W3C VCDI Integration](https://hackmd.io/@swcurran/ryZDzTbta)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-31 14:10:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2860" class=".btn">#2860</a>
            </td>
            <td>
                <b>
                    Feature: use decorators for admin api authentication
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.0.0</span>
            </td>
            <td>
                Resolves #2318 

Opening draft PR early for feedback while I work through the changes across the code (and fixing/updating/adding tests as needed).

The PR removes the authentication middleware and the logic they deal with, and implements two decorators:

- `admin_authentication`: to be used for routes that should ONLY be invoked by an administrator, such as the multitenancy endpoints, the server endpoints and so on, independently of the mode the agent is running as.
- `tenant_authentication`: to be used to require authentication by either providing a tenant token (multi-tenant mode) or a valid api-key (single-tenant mode).

Both decorators account for unauthenticated `options` requests as well as insecure mode. Insecure paths will just not be decorated. Middleware code - currently commented-out - will be removed.

I think the bit of refactoring required for this to work (including plugins once released) is well worth the flexibility - looking for early feedback especially from @dbluhm, @ianco, @jamshale 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-28 19:48:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2858" class=".btn">#2858</a>
            </td>
            <td>
                <b>
                    fix: states for discovery record to emit webhook
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds states to the the Discover Features record in order to trigger emitting webhooks containing the disclosed features to the controller. Without this change, retrieving the supported features of the remote agent is _extremely_ inconsistent. You just have to hope that the disclosure comes back in 5 seconds or try doing an exponential back off polling of the discover feature record to see if it showed up.

And a few other simplifications.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-26 18:45:29 +0000 UTC
    </div>
</div>

