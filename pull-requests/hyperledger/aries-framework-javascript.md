---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1372" class=".btn">#1372</a>
            </td>
            <td>
                <b>
                    fix(askar): custom error handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 13:28:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1370" class=".btn">#1370</a>
            </td>
            <td>
                <b>
                    feat: add oob proof proposal
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
        Created At 2023-03-07 06:53:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1369" class=".btn">#1369</a>
            </td>
            <td>
                <b>
                    feat: add support for queries by credential attribute value and marker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The PR implements the support for queries by credential attribute presence and value

**work funded by the Government of Ontario**
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 19:31:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1367" class=".btn">#1367</a>
            </td>
            <td>
                <b>
                    fix(anoncreds): Buffer not imported from core
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Subtle omission that was causing `encodeCredentialValue` to fail under React Native.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-04 23:21:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1362" class=".btn">#1362</a>
            </td>
            <td>
                <b>
                    feat(indy-vdr)!: extend did:indy support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Same changes as in #1347, but now for indy-vdr.

It updates the anoncreds registry to support both legacy and did:indy identifiers.

There's one issue that needs to be resolved, but I'd like to do that in a separate PR, is that currently the code isn't set up in a way yet that we support using both did:indy and legacy identifiers in anoncreds for _issuance_. As the holder and verifier only do resolving, it works with both now. 

What still needs to be done:
- when a credential with legacy identifiers or vice versa is received, allow it to be shared as the other format. I want to store all credentials using the new did:indy identifiers, and we can optionally transform the identifiers to legacy when needed (in the credential/proof format services)
- creating an offer for legacy format as the record always stores using the did:indy format. I'd also like to handle this in the format services, so the storage / issuer/holder/verifier services always use the new formats. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 13:26:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1361" class=".btn">#1361</a>
            </td>
            <td>
                <b>
                    test: various improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a few improvements to the test setup that should hopefully prevent timeouts, but also make sure we test the askar setup:
- only run askar related tests in node18
- add ref-napi resolution in node18
- increase timeout for some packages that often timeout
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 13:08:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1359" class=".btn">#1359</a>
            </td>
            <td>
                <b>
                    fix(tenant): Correctly configure storage for multi tenant agents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes hyperledger/aries-framework-javascript#1353
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 12:36:10 +0000 UTC
    </div>
</div>

