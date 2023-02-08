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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3521" class=".btn">#3521</a>
            </td>
            <td>
                <b>
                    feat: option to pass SD hash alg into Credential.MakeSDJWT()
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
        Created At 2023-02-08 16:08:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3520" class=".btn">#3520</a>
            </td>
            <td>
                <b>
                    chore: Add interop test for verifier
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add interop tests for verifier - this is also to prove that we will not have issues with json libraries for interop (string hardening vs. canonicalization note in spec).

Since disclosures are created by the issuer the value can be influenced by marshalling (e.g. spaces, map order etc.) however it will not influence functionality since we are not supposed to re-create disclosures at any point.

Closes #3518

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-07 21:17:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3514" class=".btn">#3514</a>
            </td>
            <td>
                <b>
                    fix: prexexch - contains check on filter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 22:39:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3513" class=".btn">#3513</a>
            </td>
            <td>
                <b>
                    chore: Add audience option to issuer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Included:
- resolve merge conflict in unit-tests between Filip's id PR and add SD-JWT to presexch PR
- add audience option to issuer
- remove irrelevant to-do(s)
- remove one integration test (was replaced by NewFromVC)
- add sha-384 to integration tests

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 21:21:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3512" class=".btn">#3512</a>
            </td>
            <td>
                <b>
                    feat: creating SD-JWT from VC will leave subject ID as regular field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                instead of turning subject ID into an SD field.

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 20:30:23 +0000 UTC
    </div>
</div>

