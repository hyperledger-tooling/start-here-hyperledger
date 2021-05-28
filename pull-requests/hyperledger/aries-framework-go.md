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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2809" class=".btn">#2809</a>
            </td>
            <td>
                <b>
                    feat: RFC0593 REST API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">aip 2.0</span>
            </td>
            <td>
                Signed-off-by: George Aristy <george.aristy@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 21:14:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2808" class=".btn">#2808</a>
            </td>
            <td>
                <b>
                    feat: JSON-LD context API bindings for mobile agent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #2805

Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 17:02:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2806" class=".btn">#2806</a>
            </td>
            <td>
                <b>
                    test: BDD tests for context API js bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * added BDD tests for js context API bindings
* removed `jsonld` section from URL path for adding context
* switched to `json.RawMessage` for `Content` field in `ContextDocument` type

Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 11:56:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2804" class=".btn">#2804</a>
            </td>
            <td>
                <b>
                    feat: API for adding JSON-LD contexts to the underlying storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
- implemented API for adding JSON-LD contexts to the underlying storage
- added new embedded contexts:
  * https://w3id.org/security/suites/bls12381-2020/v1
  * https://w3id.org/security/suites/jws-2020/v1
  * https://w3id.org/security/suites/ed25519-2018/v1
  * https://w3id.org/security/suites/x25519-2019/v1
  * https://w3id.org/security/suites/secp256k1-2019/v1
- removed contexts used for tests from core set:
  * https://www.w3.org/2018/credentials/examples/v1
  * https://www.w3.org/ns/odrl.jsonld

Bindings for mobile agent will be handled in the [follow-up ticket](https://github.com/hyperledger/aries-framework-go/issues/2805).

Closes #2730

Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 19:20:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2801" class=".btn">#2801</a>
            </td>
            <td>
                <b>
                    fix: BBS+ JWK values of crv and kty
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated as per https://w3c-ccg.github.io/ldp-bbs2020/#example-4-jwk-encoded-bls12-381-g2-key

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 14:14:56 +0000 UTC
    </div>
</div>

