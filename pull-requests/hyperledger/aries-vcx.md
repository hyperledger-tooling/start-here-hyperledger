---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/812" class=".btn">#812</a>
            </td>
            <td>
                <b>
                    Add new crates for DID parsing, DID document building, and DID resolution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">feature</span><span class="chip">skip-ci</span>
            </td>
            <td>
                This PR introduces new crates related to DID parsing, DID document building, and DID resolution, thus partially addressing issue #706 .

Some features in the added crates have no immediate use inside of AriesVCX, and we may consider moving some of these crates to a separate project, especially as the number of implemented resolvers begins to grow. However, their inclusion in the PR is due to the immediate need for a Sovrin DID method resolver, while striving to keep in line with following design goals:

* suitability for use in AriesVCX, and
* reusability in other projects, such as a driver for [universal-resolver](https://github.com/decentralized-identity/universal-resolver),
* compliance with the relevant standards and specifications:
  * [DID Core specification](https://www.w3.org/TR/did-core),
  * [DID Resolution draft](https://w3c-ccg.github.io/did-resolution),
  * [Sovrin DID method specification](https://sovrin-foundation.github.io/sovrin/spec/did-method-spec-template.html).

 The following crates have been added:

#### did_parser
This crate is responsible for parsing DID URLs and DIDs into easily queriable components, as well as DID (URL) validation. Includes `ParsedDID` and `ParsedDIDUrl` structs, which are used heavily throughout the remaining crates.

#### did_doc_builder
The `did_doc_builder` crate allows its users to construct, serialize and deserialize DID documents and their components that comply with the DID Core specification (https://www.w3.org/TR/did-core/).

#### did_resolver
This crate defines traits that should be implemented by DID resolvers of specific DID methods. For now, the traits are `DIDResolvable` and `DIDDereferenceable`.

#### did_resolver_registry
The `did_resolver_registry` is a simple crate that enables the registration of multiple DID resolvers for different DID methods at runtime and subsequent resolution of DIDs for methods with a registered resolver, thus enabling support for variable number of DID methods.

#### did_resolver_sov
This crate provides a DID resolver for the Sovrin DID method (https://sovrin-foundation.github.io/sovrin/spec/did-method-spec-template.html), and hence is the main candidate for possible use in AriesVCX.

Please review and let me know if any further changes are required.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 06:10:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/811" class=".btn">#811</a>
            </td>
            <td>
                <b>
                    removed unused constants and reformatted constants in /aries-vcx/src/utils/constant.rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - deleted unused constants from /aries-vcx/src/utils/constants.rs
- Reformatted the JSON constants to multi-line format from single-line for better readability.
- This PR is for issue #773 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-22 12:44:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/809" class=".btn">#809</a>
            </td>
            <td>
                <b>
                    Unit test for enum SerializableObjectWithState
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix: #774 
Add unit test for `serialization` and `deserialization` of enum ``SerializeableObjectWithState``.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-21 11:08:58 +0000 UTC
    </div>
</div>

