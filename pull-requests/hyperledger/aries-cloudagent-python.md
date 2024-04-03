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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2867" class=".btn">#2867</a>
            </td>
            <td>
                <b>
                    Add missing verificaiton method option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I replaced the custom `IssuanceOptionsSchema` schema on the vc/issue endpoint with the previous `LDProofOptionsSchema`. The idea will be to revisit the idea of having custom options field for different endpoints in a post 1.0 version. The verificationMethod option is necessary when issuing using unconventional did methods, such as did:web where the wallet can't correlate a verificationMethod with a specific did
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 22:44:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2866" class=".btn">#2866</a>
            </td>
            <td>
                <b>
                    Fix run_tests script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix a change that I think @dbluhm did awhile back, which is now causing issues when trying to run tests locally.

@dbluhm  what was the reason for the fix?  This PR removes your change but maybe there is an alternative that addresses your reasons without breaking local tests ...

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 18:04:59 +0000 UTC
    </div>
</div>

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

