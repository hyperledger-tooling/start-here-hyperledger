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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3566" class=".btn">#3566</a>
            </td>
            <td>
                <b>
                    perf: remove extra parsing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                verifySignature does not require parsed claims to do that functionality. we already parsing claims in many other places.
![image](https://user-images.githubusercontent.com/3065048/234279813-37d7d469-fec9-4e60-8565-ed4a40ce6903.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 12:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3565" class=".btn">#3565</a>
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
        Created At 2023-04-24 20:12:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3564" class=".btn">#3564</a>
            </td>
            <td>
                <b>
                    perf: ignore extra parsing
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
        Created At 2023-04-24 16:05:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3563" class=".btn">#3563</a>
            </td>
            <td>
                <b>
                    perf: improve parsing operations performance
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
        Created At 2023-04-22 12:15:23 +0000 UTC
    </div>
</div>

