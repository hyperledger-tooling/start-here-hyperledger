---
layout: default
title: firefly-signer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-signer
---

# firefly-signer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-signer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/4" class=".btn">#4</a>
            </td>
            <td>
                <b>
                    ABI encoder and decoder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - [x] JSON parser for ABI defintion
- [x] Modeling and verification for of all elemental types, arrays, and tuple types
  - [x] `int<M>`
  - [x] `uint<M>`
  - [x] `address`
  - [x] `bool`
  - [x] `fixed<M>x<N>`
  - [x] `ufixed<M>x<N>`
  - [x] `bytes` / `bytes<M>`
  - [x] `function`
  - [x] `string`
  - [x] `tuple`
  - [x]  fixed arrays `T[k]`
  - [x] variable arrays `T[]`
  - [x] API access to parsed type tree for features such as Swagger/OpenAPI generation
- [x] External input data mapping to ABI structure
  - [x] JSON types
  - [x] Go types
  - [x] Object style `{"arg1": 123}` input for function parameters/nested-tuples
  - [x] Array style `[123]` input for function parameters/nested-tuples
  - [x] API access to parsed value tree, mapped against type tree
- [x] ABI data encoding / serialization
   - [x] Unit tests for all examples in https://docs.soliditylang.org/en/v0.8.13/abi-spec.html 
- [ ] ABI data decoding / parsing
- [ ] JSON data serialization from value tree
- [ ] README updates
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-08 22:03:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/3" class=".btn">#3</a>
            </td>
            <td>
                <b>
                    Move to firefly-common dependency, and add config docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Moves over all dependences to `firefly-common` that are now there
- Adds `config.md` auto-generation and link from `README.md`

Depends on (go.mod pulls these in directly):
- https://github.com/hyperledger/firefly-common/pull/4

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 12:25:02 +0000 UTC
    </div>
</div>

