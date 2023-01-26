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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3498" class=".btn">#3498</a>
            </td>
            <td>
                <b>
                    feat: SD-JWT: Add option for non-selectively disclosable claims (issuer)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                From spec: The Issuer may also make certain claims or sub-claims non-selectively disclosable. 

Added option WithNonSelectivelyDisclosableClaims() for specifying non-selectively disclosable claims to issuer.

Closes: #3497

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-25 21:07:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3496" class=".btn">#3496</a>
            </td>
            <td>
                <b>
                    feat: method to marshal SD-JWT VC in combined format for presentation
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
        Created At 2023-01-25 07:32:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3495" class=".btn">#3495</a>
            </td>
            <td>
                <b>
                    fix: Move cnf and _sd_alg to vc level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move cnf and _sd_alg from credential subject level to vc level

Closes #3494

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-24 21:06:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3493" class=".btn">#3493</a>
            </td>
            <td>
                <b>
                    feat: verifiable.ParseCredential() supports combined SD-JWT credentials
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
        Created At 2023-01-24 17:45:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3492" class=".btn">#3492</a>
            </td>
            <td>
                <b>
                    feat: SD-JWT: Add NewFromVC to Issuer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pass VC into NewFromVC and the issuer will create selective disclosures for everything in vc->credential subject and add the fields from options.

Closes #3491


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-24 13:57:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3490" class=".btn">#3490</a>
            </td>
            <td>
                <b>
                    chore: Support verification of 'vc' claims with holder binding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Support verification of 'vc' claims with holder binding

Closes #3489

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-23 20:50:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3488" class=".btn">#3488</a>
            </td>
            <td>
                <b>
                    chore: Integration test for structured claim option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added integration test for structured claim option.

Closes #3487

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-20 17:31:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3486" class=".btn">#3486</a>
            </td>
            <td>
                <b>
                    fix: presex desctiptor format.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>

**Title:**
Fix for Presentation Exchange descriptor format

**Description:**
[Link to the GitHub issue it solves (if any)]

**Summary:**

Presentation Exchange creates verifiable presentations with presentation submission descriptors with invalid format value.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-20 15:44:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3485" class=".btn">#3485</a>
            </td>
            <td>
                <b>
                    fix: Release claims by claim disclosure not by claim name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently the holder releases disclosures based on claim name. If we have same name in different objects within claims this will not work.

Closes #3484

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 19:08:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3483" class=".btn">#3483</a>
            </td>
            <td>
                <b>
                    chore: SD-JWT: Support claims with 'vc' verification in issuer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change logic for resolving _sd_alg to look for _sd_alg in the following path:
1. claims top level (as per spec)
2. claims -> vc -> credential subject (in case that it is not present at claims top level)

Closes #3482

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 14:54:44 +0000 UTC
    </div>
</div>

