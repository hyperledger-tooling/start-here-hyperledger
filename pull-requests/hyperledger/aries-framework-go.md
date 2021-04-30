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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2772" class=".btn">#2772</a>
            </td>
            <td>
                <b>
                    Add public key fetcher for validating the verifiable credential.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Add PublicKeyFetcher for validating the verifiable credential.

**Description:**
#1316 

**Summary:**
Previously, since there was no PulicKeyFetcher, there was no way to separately validate a Validate Credential, but it can be verified by adding PublicKeyFetcher.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 02:43:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2771" class=".btn">#2771</a>
            </td>
            <td>
                <b>
                    feat: vc wallet command controller for managing profiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added create & update profile command controllers
- Part of #2770

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 23:50:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2769" class=".btn">#2769</a>
            </td>
            <td>
                <b>
                    feat: apis to create keys in wallet kms
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                -EDV encryption & MAC key IDs cannot be passed as profile settings for
localkms users since wallet creates local kms internally based on user's
secret lock service. So wallet has to expose an API to generate EDV keys
in wallet kms.
- Closes #2768

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 19:11:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2767" class=".btn">#2767</a>
            </td>
            <td>
                <b>
                    fix: ECDH-1PU key derivation logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                and add ECDH-1PU test against the draft's test vector

closes #2766

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 18:18:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2764" class=".btn">#2764</a>
            </td>
            <td>
                <b>
                    feat: wallet open options for webkms & EDV
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added more unlock wallet options to use all aries webkms & EDV
customization opts.
- can be used to pass auth & authz based http headers for EDV & web kms
- closes #2763

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 21:44:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2760" class=".btn">#2760</a>
            </td>
            <td>
                <b>
                    refactor: cleanup JSON-LD contexts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR:
* simplifies new JSON-LD document loader:
  - support for `WithContextFS` was removed (in practice it didn't justify itself)
  - "core" set of embedded contexts was defined (extra contexts can be preloaded using `WithExtraContexts`)
* replaces the following contexts:
  - `https://trustbloc.github.io/context/vc/credentials-v1.jsonld` -> `https://w3id.org/security/jws/v1`
  - `https://trustbloc.github.io/context/vc/examples-v1.jsonld` -> `https://w3id.org/vc-revocation-list-2020/v1` (only in BDD tests - this allows to remove it from the main embedded set)

Closes #2751

Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-27 10:57:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2759" class=".btn">#2759</a>
            </td>
            <td>
                <b>
                    feat: vc wallet EDV storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - if wallet user provides EDV settings during profile creation for
storage then wallet will create internal EDV client instance for storing
wallet contents
- for now, encryption and MAC key IDs has to be provided by client user
during profile creation/update
- closes #2757

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 22:46:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2755" class=".btn">#2755</a>
            </td>
            <td>
                <b>
                    fix: presentation-exchange schema.uri matching
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">aip 2.0</span><span class="chip">bug</span>
            </td>
            <td>
                The `schema.uri` in presentation definitions should be the full URI to the type's definition (jsonschema or jsonld), not just the context. [Reference](https://github.com/decentralized-identity/presentation-exchange/issues/134#issuecomment-721624167).

TODO - #2756 

Signed-off-by: George Aristy <george.aristy@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 15:13:52 +0000 UTC
    </div>
</div>

