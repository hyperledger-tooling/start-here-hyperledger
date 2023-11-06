---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2591" class=".btn">#2591</a>
            </td>
            <td>
                <b>
                    Goal and Goal Code in invitation URL.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a unit test to ensure goal/goal code are in the encoded invitation URL.

Fixes #2583 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 23:23:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2590" class=".btn">#2590</a>
            </td>
            <td>
                <b>
                    Fix Issue #2589 TypeError When There Are No Nested Requirements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added `if` statement, same as in calling function `create_vp`, to the called function `apply_requirements`. Since the former calls `apply_requirements` in both cases (`if req.nested_req` or not), the called function should handle both cases as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 18:49:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2588" class=".btn">#2588</a>
            </td>
            <td>
                <b>
                    Anoncreds rs - draft PR to monitor differences between the branch and main
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
        Created At 2023-11-02 16:25:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2587" class=".btn">#2587</a>
            </td>
            <td>
                <b>
                    feat: use a local static cache for commonly used contexts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.11.0</span>
            </td>
            <td>
                [Related to this issue](https://github.com/hyperledger/aries-cloudagent-python/issues/2581)

* Package a list of commonly used contexts 
* Replace the context loader from pyld with `StaticCacheJsonLdDownloader`
* `StaticCacheJsonLdDownloader` resolves contexts from local package in priority, then delegates to a downloader
* As of now, `JsonLdDocumentDownloader` and `JsonLdDocumentParser` are simply lifted from pyld in a way that decouples downloading and parsing JSON-LD documents.
* Tests are mostly drafts, waiting for feedback before investing time there.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 12:57:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2585" class=".btn">#2585</a>
            </td>
            <td>
                <b>
                    Another catchup from main 
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
        Created At 2023-11-01 21:28:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2584" class=".btn">#2584</a>
            </td>
            <td>
                <b>
                    Dockerfile.indy - Include aries_cloudagent code into build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2582 

Need to have the `poetry` install load `aries-cloudagent` module. So add the source to the image and change the install command to load it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-01 19:33:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2578" class=".btn">#2578</a>
            </td>
            <td>
                <b>
                    feat: emit did:peer:2 in DID Exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements did:peer:2 support for DID Exchange. If the `--emit-did-peer-2` flag is set, ACA-Py will create and send a did:peer:2 DID instead of an unqualified DID and an attached Document in DID Exchange messages.

This PR also implements the `did_rotate~attach` from the [proposed DID Exchange v1.1](https://github.com/hyperledger/aries-rfcs/pull/795). It will include the `did_rotate~attach` attribute on responses when relevant and will expect to receive them on responses as well.

To achieve this, the following changes were made:
- Add `wallet.create_key`. `create_key` is just a more generic `create_signing_key`. Literally no difference in implementation; it just seemed an inappropriate name for how it was being used. I can be convinced that we should not do this.
- Add `wallet.store_did`. This enables us to more easily create DIDs outside of the wallet. The `wallet.create_local_did` method is starting to get a bit complicated. Rather than shoehorning all DID creation into the wallet interface, I think it makes sense to transition to a system where the wallet creates the primitives (such as keys) but then the creation of the DID itself is performed outside of the wallet. This was especially necessary because, in order to create a did:peer:2, we also need service info which can differ per connection (mediation used or not, for instance) and the wallet is simply not aware of the concept of services nor the context of the connection and associated mediation records. As part of an early pass, I even went as far as to introduce a DID Registration interface (which makes this attempt perhaps my third one in recent memory). I continue to struggle to create an interface that is generic enough to enable registering DIDs using plugged in registrars but still actually be useful. The requirements between methods varies so widely that the interface becomes nearly useless (at least in the context of ACA-Py). I'm finding it more reasonable to simply call a specific "registrar" directly. In these changes for did:peer:2, this is simply calling into the did-peer-2 library's `generate` method.
- Add `--emit-did-peer-2` flag and associated setting.
- Add support for easily creating an attachment with `text/string` mime type, as is used in the `did_rotate~attach`.
- Add the `PEER2` DID Method definition

Opening as a draft since, at the time of opening, this hasn't been thoroughly exercised by tests yet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 03:24:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2577" class=".btn">#2577</a>
            </td>
            <td>
                <b>
                    Send Problem report when CredEx not found
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #2549 

Address the situation when an issuer sends an offer and then deletes that offer (credential exchange) before the holder accepts it. When this is an `indy` credential exchange, a Problem Report is sent; when this is a `json-ld` exchange, the holder's accept actually becomes an unbound request for the credential and the flow carries on.

A discussion is warranted to see if we want to implement something more global? Seems like at any point in any protocol one side may not find their record and the other side should be notified of the abandonment. Maybe it is already done and this was just a gap...

Added BDD tests to address the deletion and followup acceptance for `indy` and `json-ld` and also the holder sending a request for credential to issuer. Again, `indy` is not allowed, `json-ld` can flow into a credential issuance.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 01:11:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2576" class=".btn">#2576</a>
            </td>
            <td>
                <b>
                    0.11.0-rc1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-30 22:07:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2575" class=".btn">#2575</a>
            </td>
            <td>
                <b>
                    0.11.0-rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-30 20:30:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2573" class=".btn">#2573</a>
            </td>
            <td>
                <b>
                    chore: point to official sd-jwt lib release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adjusts the version of sd-jwt pulled to be the official release now published to PyPI: https://pypi.org/project/sd-jwt/
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-30 19:07:54 +0000 UTC
    </div>
</div>

