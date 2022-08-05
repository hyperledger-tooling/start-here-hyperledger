---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3315" class=".btn">#3315</a>
            </td>
            <td>
                <b>
                    feat: Add jwt-vc test suites supporting AFGO
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mykhailo Sizov <mykhailo.sizov@securekey.com>

**Title:**
Add jwt-vc test suites supporting AFGO

**Description:**
https://github.com/hyperledger/aries-framework-go/issues/3288

**Summary:**
Added signer and verifier based on private/public key type.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 13:37:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3313" class=".btn">#3313</a>
            </td>
            <td>
                <b>
                    fix: change aries default wallet to didcommwallet.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>

**Title:**
Change aries default wallet to didcommwallet.

**Summary:**

Didcomm functionality was moved from vcwallet to didcommwallet, to agent-sdk work properly default wallet should be changes to didcommwallet.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 12:16:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3312" class=".btn">#3312</a>
            </td>
            <td>
                <b>
                    feat: support of presentation exchange v2.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>


**Title:**
Presentation exchange v2

**Description:**
https://github.com/hyperledger/aries-framework-go/issues/3297

**Summary:**

Added support of changes from the latest presentation exchange draft https://identity.foundation/presentation-exchange/


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 12:29:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3309" class=".btn">#3309</a>
            </td>
            <td>
                <b>
                    refactor: credential manifest enhancements to match wallet-rendering specs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
**Summary:**

- Refactored credentialmanifest.go 
  - moved everything related to resolving the different types into a separate file called resolve.go to make it clearer as to what is coming from the credential manifest and wallet rendering specs and what is needed for displaying 
  - moved common functions to common.go
- Changes to match specs:
  - Fixed display mapping object to use text property if paths is empty 
    - validateDisplayMappingObject to check for if both the text field and the paths field is empty
    - update unit tests for this
  - ValidateCredentialApplication 
    - Added check for case where manifest's format is empty but credential application's is not (credential application's formats should be a subset of credential manifest's)
    - Removed duplicate code for checking credential application against credential manifest
    - update unit tests
  - Added missing optional property to CredentialFulfillment
  - Added missing optional properties to schema format

Closes #3304 
Closes #3274 
Closes #3280 
Closes #3281
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 18:26:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3308" class=".btn">#3308</a>
            </td>
            <td>
                <b>
                    fix: move resolve credential manifest from didcommwallet to vcwallet.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>

**Title:**
Move ResolveCredentialManifest from didcommwallet to vcwallet.

**Summary:**

ResolveCredentialManifest is related to vcwallet.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 07:01:04 +0000 UTC
    </div>
</div>

