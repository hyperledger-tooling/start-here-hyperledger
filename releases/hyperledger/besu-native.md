---
layout: default
title: besu-native
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu-native
---

# besu-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.9.0
                </span>
            </td>
            <td>
                # Release 0.9.0
This release bumps besu native to java 21.  Creating a release and tag for 0.9.0, which includes accumulated changes in intervening versions since 0.6.1.  

* implement EIP-196 and EIP-2537 using gnark-crypto, bump to java 21, gradle 8.8 [#168](https://github.com/hyperledger/besu-native/pull/168)

## Binaries
[altbn128-0.9.0.jar](https://hyperledger.jfrog.io/hyperledger/besu-maven/org/hyperledger/besu/altbn128/0.9.0/altbn128-0.9.0.jar) / sha 0be2fed2cca08a1fec2195baa1ba3506e42427647c795651e39355c8b92bccb7
[arithmetic-0.9.0.jar](https://hyperledger.jfrog.io/hyperledger/besu-maven/org/hyperledger/besu/arithmetic/0.9.0/arithmetic-0.9.0.jar) / sha 90b0af5d0e046b0ff912f520dfa0c7288b43c37564982b2c337d72c66cf33c7e
[blake2bf-0.9.0.jar](https://hyperledger.jfrog.io/hyperledger/besu-maven/org/hyperledger/besu/blake2bf/0.9.0/blake2bf-0.9.0.jar) / sha c553879bac7769c6f02d0bcad8e4fc44eabbcee4d24a834da5cb1b09382c1283
[bls12-381-0.9.0.jar](https://hyperledger.jfrog.io/hyperledger/besu-maven/org/hyperledger/besu/bls12-381/0.9.0/bls12-381-0.9.0.jar) / sha 516b7e6ede5bf043fb2b786672cf92d751e1b475f6de9e598f8c713b3a083143
[gnark-0.9.0.jar](https://hyperledger.jfrog.io/hyperledger/besu-maven/org/hyperledger/besu/gnark/0.9.0/gnark-0.9.0.jar) / sha 2396af3f4a3bf938351c0fcae344d1ed266acb803dffb5699ca332d204e91747
[ipa-multipoint-0.9.0.jar](https://hyperledger.jfrog.io/hyperledger/besu-maven/org/hyperledger/besu/ipa-multipoint/0.9.0/ipa-multipoint-0.9.0.jar) / sha 62996e282ac986c82cd6eab11f41ee4fc8dd42ca98189962f3d5cf0606b3fe99
[secp256k1-0.9.0.jar](https://hyperledger.jfrog.io/hyperledger/besu-maven/org/hyperledger/besu/secp256k1/0.9.0/secp256k1-0.9.0.jar) / sha 8f69dabd90e345b7bacbbeda58764d80d9fdbc3704c964fc8fa54a8cb7e751e7
[secp256r1-0.9.0.jar](https://hyperledger.jfrog.io/hyperledger/besu-maven/org/hyperledger/besu/secp256r1/0.9.0/secp256r1-0.9.0.jar) / sha 3d4c1553c907a590a668a26d17f3d23630ba456442f2812653439d70e030069d

## Accumulated change from prior versions
### 0.6.2 - 0.8.5
* ipa-multipoint : add verkle proof verification (#169)
* BLS12-381: Add subgroup checks to BLS-12 mul amd multiexp precompiles (#166)
* ipa-multipoint : Use debug-like to log the execption from the ffi::commit_to_scalars (#161)
* ipa-multipoint : Error handling and init no-copy in JNI (#158)
* ipa-multipoint : Removes pedersenHash method (#157)
* ipa-multipoint : Updates rust-verkle dependency (#156)
* ipa-multipoint : add update sparse commitment (#149)
* ipa-multipoint : add groupToField and return uncompressed serialized commitments (#146)
* ipa-multipoint : switch to LE bytes (#145)
* ipa-multipoint : update to a version of rust-verkle which uses little endian ipa-multipoint (#143)
* ipa-multipoint : Switch to `ffi_interface` ipa-multipoint (#139)
* ipa-multipoint : Modify test vectors to use canonical scalars for their input  (#142)
* ipa-multipoint : fix commit for verkle trie library(#141)
* ipa-multipoint : Fix linking error for LibIpaMultipoint(#131)
* add support for Mimc on bls12-377 [#132](https://github.com/hyperledger/besu-native/pull/132)
* FIX: javadoc issues [#125](https://github.com/hyperledger/besu-native/pull/125)
* ENH: adds ipa-multipoint library with Pedersen primitives [#123](https://github.com/hyperledger/besu-native/pull/123)
* Bump github.com/consensys/gnark-crypto in /gnark/gnark-jni [#122](https://github.com/hyperledger/besu-native/pull/122)
* Add k1 normalize signature method to secp256k1 [#118]](https://github.com/hyperledger/besu-native/pull/118)
* Handle incomplete input on modExp correctly [#114]](https://github.com/hyperledger/besu-native/pull/114)
* Add mimc/gnark library [#106](https://github.com/hyperledger/besu-native/pull/106)
* Change module names from `native` to `nativelib` [#108](https://github.com/hyperledger/besu-native/pull/108)
* Use Aurora's modexp implementation in arithmetic [#111](https://github.com/hyperledger/besu-native/pull/111)
* Add new "arithmetic" library to support basic (but expensive) arithmetic [#98](https://github.com/hyperledger/besu-native/pull/98)
* support computing proof with n arguments [#89](https://github.com/hyperledger/besu-native/pull/89)
* Java modules support [#90](https://github.com/hyperledger/besu-native/pull/90)
* Add CodeQL workflow for GitHub code scanning [#92](https://github.com/hyperledger/besu-native/pull/92)

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-native/releases/tag/0.9.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-06-25 19:31:07 +0000 UTC
    </span>
</div>

