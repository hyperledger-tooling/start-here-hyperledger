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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3561" class=".btn">#3561</a>
            </td>
            <td>
                <b>
                    chore: update afgo with transitive component dependencies.
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
        Created At 2023-04-20 15:40:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3560" class=".btn">#3560</a>
            </td>
            <td>
                <b>
                    chore: update go mod files to latest version of new components.
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
        Created At 2023-04-20 14:25:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3559" class=".btn">#3559</a>
            </td>
            <td>
                <b>
                    fix: Match submission requirements not apply limited disclosure.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**

MatchSubmissionRequirement no longer applies limited disclosure on its results, now it just filters applicable credentials.

**Summary:**

Functionality that applies limited disclosure was factored from `filterConstraints` to separate function limitDisclosure.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 08:40:26 +0000 UTC
    </div>
</div>

