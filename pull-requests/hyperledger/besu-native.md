---
layout: default
title: besu-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-native
---

# besu-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/153" class=".btn">#153</a>
            </td>
            <td>
                <b>
                    Refactor/ipa multipoint interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR initialise a refactor of the JNI/FFI_interface to standardize the interfaces between Java and Rust.

Notably, we want to leverage only crypto-primitives related to vector commitments from rust-verkle.
Any verkle logic is for besu-verkle-tries.
Moreover, methods are composable since they follow a uniform format.

Here are the new features:

- Inputs and outputs between java and rust are rlp-encoded with all values being little-endian bytes.
- types module includes 3 types: CommitmentBytes, CommitmentBytesCompressed, ScalarBytes. These are the only primitives that are used by the ffi-interface.
- convert modules implements conversions to and from rust-verkle types.
- encoding/decoding modules implements rlp Decodable and Encodable for our types.
- traits module includes Committable and Updatable for vector commitments functionalities.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 11:36:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Add prover and verifier calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Will wait for https://github.com/hyperledger/besu-native/pull/151 and/or changes to pedersenHash before asking for review on this
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-26 17:19:20 +0000 UTC
    </div>
</div>

