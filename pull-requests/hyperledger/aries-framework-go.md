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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3481" class=".btn">#3481</a>
            </td>
            <td>
                <b>
                    feat: Add structured claims option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added:
- structured claims option to issuer
- verify digests in structured claims for holder
- structured claims processing to verifier

Closes #3478

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 16:15:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3480" class=".btn">#3480</a>
            </td>
            <td>
                <b>
                    chore: Create SD-JWT without signature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add test for creating SD-JWT without signature.

Closes #3479

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 21:03:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3477" class=".btn">#3477</a>
            </td>
            <td>
                <b>
                    chore: Rename DisclosureSeparator to CombinedFormatSeparator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Clean-up task:

- rename DisclosureSeparator to CombinedFormatSeparator
- move issuer Payload struct from common to issuer package

Closes #3476

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 18:12:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3475" class=".btn">#3475</a>
            </td>
            <td>
                <b>
                    feat: SD-JWT Verifier: Verify Holder Binding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If Holder Binding is required, verify that the Holder Binding JWT is signed by the Holder and valid.

Closes #3471

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 21:47:56 +0000 UTC
    </div>
</div>

