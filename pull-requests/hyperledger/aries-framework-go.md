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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3136" class=".btn">#3136</a>
            </td>
            <td>
                <b>
                    feat: credential manifest support in vcwallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added new resolve credential manifest interface to resolve
fulfillments and credentials
- refactores testdata files to avoid duplicate testdata files across
various packages
- Closes #3120

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-22 19:51:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3135" class=".btn">#3135</a>
            </td>
            <td>
                <b>
                    feat: credential manifest resolve - specify schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - specify schema along with resolved values which will be helpful for
rendering resolved values

- Part of #3092

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 01:30:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3134" class=".btn">#3134</a>
            </td>
            <td>
                <b>
                    Add option to enable remote document loading for mobile bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                when enabled, documents that are not available locally will be fetch remotely for mobile bindings.

Does replace pull request #3053.

Signed-off-by: Michel Sahli <michel.sahli@adnovum.ch>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 11:30:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3133" class=".btn">#3133</a>
            </td>
            <td>
                <b>
                    test: WACI Issuance BDD tests for Go SDK
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
        Created At 2022-01-20 01:03:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3132" class=".btn">#3132</a>
            </td>
            <td>
                <b>
                    feat: add pthid to the didcomm v2 message replying to an oobv2 invitation
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
        Created At 2022-01-19 21:39:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3131" class=".btn">#3131</a>
            </td>
            <td>
                <b>
                    fix: smooth out behaviour of version-agnostic didcomm models
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
        Created At 2022-01-19 06:36:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3130" class=".btn">#3130</a>
            </td>
            <td>
                <b>
                    feat: Export Credential Manifest and Output Descriptor validate methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reworked the existing Credential Manifest and Output Descriptor validation methods so that they can be called directly outside of the cm package without requiring json.Unmarshal to be called. This gives callers more flexibility and supports more use cases.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 21:23:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3129" class=".btn">#3129</a>
            </td>
            <td>
                <b>
                    feat: credential manifest resolve - support for arbitrary type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Part of #3092

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-18 03:31:27 +0000 UTC
    </div>
</div>

