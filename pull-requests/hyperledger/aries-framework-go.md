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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3107" class=".btn">#3107</a>
            </td>
            <td>
                <b>
                    fix: issuecredential empty metadata request should not override default message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 22:05:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3105" class=".btn">#3105</a>
            </td>
            <td>
                <b>
                    refactor: update goal_code invalid name for OOB V2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 21:42:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3104" class=".btn">#3104</a>
            </td>
            <td>
                <b>
                    chore: upgrade to Go 1.17 and fix MacOS Monterey Go Bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 16:08:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3102" class=".btn">#3102</a>
            </td>
            <td>
                <b>
                    feat: Method to add Credential Fulfillment to Verifiable Presentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added method to add Credential Fulfillment to an existing Verifiable Presentation.
- Also added https://identity.foundation/credential-manifest/fulfillment/v1 to test contexts for JSON-LD document loader.
- Renamed existing sample data as needed for consistency with the new sample data added in this commit and existing sample data.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 20:01:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3101" class=".btn">#3101</a>
            </td>
            <td>
                <b>
                    feat: webredirectinfo support in issue credential protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added support for webredirect info for issue credential, decline
proposal & decline request steps.
- added SDK & controller bdd tests
- Closes #3099

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 18:14:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3100" class=".btn">#3100</a>
            </td>
            <td>
                <b>
                    feat: Shorten credentialmanifest package name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 18:13:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3098" class=".btn">#3098</a>
            </td>
            <td>
                <b>
                    chore: update maintainers list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Troy Ronda <troy@troyronda.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 15:57:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3097" class=".btn">#3097</a>
            </td>
            <td>
                <b>
                    fix: Changes to Credential Application to align with spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Removed the nested Presentation Submission object from the Credential Application object
- The CredentialApplication struct is now just the ID, ManifestID, and Format properties - there is no longer a nested credential_application field
- Added a comment clarifying where/how the CredentialApplication is used

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 15:49:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3095" class=".btn">#3095</a>
            </td>
            <td>
                <b>
                    fix: removing item tagged by collection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fixing issue with `wallet.Remove()` where mapping data with collection
wasn't deleted.
- Part of #2433

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 16:51:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3093" class=".btn">#3093</a>
            </td>
            <td>
                <b>
                    fix: remote kms create keystore response format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>

**Title:**
Fix remote kms create keystore response format

**Description:**
Change type of Capability field in createKeyStoreResp to  []byte from string

**Summary:**

[Include a brief summary of your changes]


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 10:47:47 +0000 UTC
    </div>
</div>

