---
layout: default
title: web3j
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/web3j
---

# web3j <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/web3j){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j/pull/2079" class=".btn">#2079</a>
            </td>
            <td>
                <b>
                    Make getABI_* calls in wrapper should be static
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
getABI_* call in wrapper should be static method. we do not need an instance of wrapper to encode function

### Where should the reviewer start?
All files

### Why is it needed?
we do not need an instance of wrapper to encode function

## Checklist

- [x] I've read the contribution guidelines.
- [x] I've added tests (if applicable).
- [ ] I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-16 03:32:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j/pull/2076" class=".btn">#2076</a>
            </td>
            <td>
                <b>
                    Updated TypeReference and TypeDecoder to support decoding of dynamic structs and dynamic struct arrays without a priori Class definitions.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - **Updated TypeReference object to support nested types to support truly dynamic stucts.**
- **Support decoding of DynamicArray of DynamicStruct (with corresponding unit test). Change visibility of TypeReference's innerTypes and getSubTypeReference() to protected/public to allow for overriding in anonymous classes. Redo naming of some innerType-specific functions in TypeDecoder to minimize code diffs.**

### What does this PR do?
This PR builds off of the PR originally created by calmacfadden at https://github.com/hyperledger/web3j/pull/2023.

### Where should the reviewer start?
* Look in TypeDecoder.java, with attention to the decodeDynamicParameterFromStructWithTypeReference() and
decodeDynamicStructElementsFromInnerTypes(). Note that the Ctor() version of functions from PR 2023 have been
renamed to omit the Ctor so as to match the name in the main branch and reduce code diffs.

* The unit test testArrayOfDynamicStruct() provides an example of decoding an array of dynamic structs (uint256,bool,string)[]
based on a transaction from the Treasure Ruby testnet.

* I've taken some stylistic liberty by renaming TypeReference.innerTypeReferences() to TypeReferences.innerTypes().

* I've changed the scope of some fields in TypeReference from private to protected/public to allow for creating the
anonymous DynamicArray class seen in testArrayOfDynamicStruct().

### Why is it needed?
As with PR 2023, it would be useful to decode dynamic structs without having to explicitly define a corresponding class.

## Checklist

- [x] I've read the contribution guidelines.
- [x] I've added tests (if applicable).
- [ ] I've added a changelog entry if necessary.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-10 08:16:51 +0000 UTC
    </div>
</div>

