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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3391" class=".btn">#3391</a>
            </td>
            <td>
                <b>
                    feat: Add did configuration client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Did configuration client will:
- retrieve did configuration from domain
- verify requested did and domain against did configuration

Closes #3390

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-29 16:38:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3389" class=".btn">#3389</a>
            </td>
            <td>
                <b>
                    fix: Service type property MUST be a string or a set of strings.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Service type property MUST be a string or a set of strings.

Closes #3383

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 17:04:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3388" class=".btn">#3388</a>
            </td>
            <td>
                <b>
                    fix: don't panic on malformed proof properties
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Do not panic when creating new Proof object with string map that contains invalid interfaces

**Description:**
This PR fixes #3384 by guarding the type assertion in `proof.stringEntry()` and returning the empty string if it fails.

**Summary:**
Updated `proof.stringEntry()` so that the empty string is returned if the type assertion for `entry.(string)` fails (precedent from [`did.stringEntry()`](https://github.com/hyperledger/aries-framework-go/blob/main/pkg/doc/did/doc.go#L1039-L1049)). Previously, this function would panic if the provided interface was not either `nil` or a `string`.

Added unit testing to ensure that all options passed through `proof.stringEntry()` by `proof.NewProof()` can handle invalid interfaces without a panic.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-26 15:11:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3387" class=".btn">#3387</a>
            </td>
            <td>
                <b>
                    chore: Add interop did configuration test (MS)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add MS interop test for did configuration.

https://did.rohitgulati.com/.well-known/did-configuration.json

Closes #3386

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-26 15:02:05 +0000 UTC
    </div>
</div>

