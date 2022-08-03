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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3307" class=".btn">#3307</a>
            </td>
            <td>
                <b>
                    feat: Remove warning from secret lock and update documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removed a warning that would happen if trying to read in a master key using raw bytes, as this is actually a normal scenario. Also updated some related documentation to make it more clear that raw byte master keys are an expected use case.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 20:45:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3306" class=".btn">#3306</a>
            </td>
            <td>
                <b>
                    feat: Adding sqlite to mobile agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Adding sqlite to mobile agent

**Description:**
I created a component in the mobile agent that allows a user to use a storage provider that connects with SQLite.

**Summary:**

Using https://github.com/hyperledger/aries-framework-go-ext/blob/main/component/storage/mysql/store.go as reference I created a store provider that connects with SQLite. 
Also, I implemented the TotalItems() method inside the storage wrapper.

@DRK3, @sudeshrshetty, What do you think?

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 16:53:32 +0000 UTC
    </div>
</div>

