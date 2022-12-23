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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3457" class=".btn">#3457</a>
            </td>
            <td>
                <b>
                    chore: expose didsignjwt.ResolveSigningVM as a helper API
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
        Created At 2022-12-22 22:17:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3456" class=".btn">#3456</a>
            </td>
            <td>
                <b>
                    wip: Add SD-JWT Verifier (Flat)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Parse and verify combined presentation from issuer.

Closes #3455

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-22 19:11:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3454" class=".btn">#3454</a>
            </td>
            <td>
                <b>
                    feat: Add SD-JWT Holder (Flat)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Parse and verify combined presentation from issuer.

Closes #3453

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 15:42:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3452" class=".btn">#3452</a>
            </td>
            <td>
                <b>
                    feat: Add SD-JWT Issuer (Flat)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add SD-JWT Issuer (flat, no optional features).

Closes #3451

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 00:48:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3450" class=".btn">#3450</a>
            </td>
            <td>
                <b>
                    feat: enable ed25519 in jwkkid.BuildJWK()
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
        Created At 2022-12-19 19:47:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3449" class=".btn">#3449</a>
            </td>
            <td>
                <b>
                    fix: did service endpoint bug.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Volodymyr Kubiv <volodymyr.kubiv@euristiq.com>

**Title:**
Fix bug that causes incorrect serialization of did document with service endpoint property.


**Summary:**

Storing in Endpoint.rawObj not only array from origin property whole serviceEndpoint object.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 09:49:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3447" class=".btn">#3447</a>
            </td>
            <td>
                <b>
                    refactor: Minimize VDResolver interface needed for did config validate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently, the DID config validate functionality has an option for injecting in a VDR, however most of the methods in the interface are not actually used.

This change switches the option to use a minimal version of that interface that is itself a subset of the full VDR interface. With this change, a caller can now use the VDR option with a more minimal implementation that only has a Resolve method. The minimal interface still lines up with the larger VDR interface, so another caller can still use a full VDR interface implementation without making any changes.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 18:51:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3446" class=".btn">#3446</a>
            </td>
            <td>
                <b>
                    chore: DID Config Client is not passing options to DID Config API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                DID Config Client is not passing options to DID Config API 
Current unit tests are using did:key so add unit test with did resolver option

Closes #3445

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 18:00:30 +0000 UTC
    </div>
</div>

