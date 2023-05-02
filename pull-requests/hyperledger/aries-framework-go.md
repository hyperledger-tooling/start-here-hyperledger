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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3578" class=".btn">#3578</a>
            </td>
            <td>
                <b>
                    chore: update component/models for transitive dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 18:07:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3577" class=".btn">#3577</a>
            </td>
            <td>
                <b>
                    fix: invalid creds IDs returned from match submission requirements.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
**Title:**
Fix invalid creds IDs returned from MatchSubmissionRequirement.

**Summary:**

Credential returned MatchSubmissionRequirement had IDs with some random prefix. Now this is fixed.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 12:30:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3574" class=".btn">#3574</a>
            </td>
            <td>
                <b>
                    Switch to using mathlib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Use [mathlib](https://github.com/IBM/mathlib) as the implementation for elliptic curve operations.

**Description:**
This PR is an implementation of this [proposal](https://github.com/hyperledger/aries-framework-go/issues/3575).

**Summary:**

This PR changes the dependency used to handle the operations on elliptic curves needed by the BBS+ implementation. Instead of directly using the [kilic](https://github.com/kilic/bls12-381) implementation. we recommend switching to [mathlib](https://github.com/IBM/mathlib): mathlib is a module that exposes a common set of API backed by a number of different libraries ([amcl](https://github.com/hyperledger/fabric-amcl), [ConsenSys/gnark-crypto](https://github.com/ConsenSys/gnark-crypto) and [kilic](https://github.com/kilic/)). It currently supports the following curves: [FP256BN](https://neuromancer.sk/std/other/Fp256BN), [BN254](https://neuromancer.sk/std/bn/bn254), [BLS12_377](https://neuromancer.sk/std/bls/BLS12-377) and [BLS12_381](https://neuromancer.sk/std/bls/BLS12-381) (the latter in two different variants, standard and BBS compliant). mathlib is already being used by [fabric](https://github.com/hyperledger/fabric), the [idemix](https://github.com/IBM/idemix/) implementation used by fabric, the [fabric token sdk](https://github.com/hyperledger-labs/fabric-token-sdk) and the [fabric smart client](https://github.com/hyperledger-labs/fabric-smart-client).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 07:01:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3573" class=".btn">#3573</a>
            </td>
            <td>
                <b>
                    feat: support for optional field in presexch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #3572

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 20:29:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3571" class=".btn">#3571</a>
            </td>
            <td>
                <b>
                    chore: update internal dependencies to latest component changes.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 14:33:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3570" class=".btn">#3570</a>
            </td>
            <td>
                <b>
                    fix: now get submission requirements can apply SD on result VCs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Now get submission requirements can apply SD on result VCs


**Summary:**

The option is added to MatchSubmissionRequirement that allows to apply selective disclosure to resulting VCs.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 11:13:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3568" class=".btn">#3568</a>
            </td>
            <td>
                <b>
                    feat: new component for data models - DIDs, signatures, JSON-LD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                component/models/:
 - did: afgo's DID and DID Doc models.
 - ld: JSON-LD support - data models, context stores, LD-Proofs, canonicalization, etc.
 - signature: signing APIs used in DID Docs etc.
 - util: utility data models needed for other model implementations, but not specific to a given model.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 19:45:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3567" class=".btn">#3567</a>
            </td>
            <td>
                <b>
                    Revert "feat: new component for data models - DIDs, signatures, JSON-LD"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverts hyperledger/aries-framework-go#3565

PR commit had commit message and authorship broken due to a rebase, will re-push corrected
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 19:43:17 +0000 UTC
    </div>
</div>

