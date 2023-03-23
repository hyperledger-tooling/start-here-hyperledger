---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Release 0.53.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.53.0
                </span>
            </td>
            <td>
                # Changelog

## [0.53.0](https://github.com/hyperledger/aries-vcx/tree/0.53.0) (2023-03-22)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.52.0...0.53.0)

# global
* Update readme files by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/757

# aries-vcx

### Breaking changes
* Prover APIs:
  * Proof verifier: add `get_revocation_status` method by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/769
* Verifier APIs:
  * Rename prover methods, extend test test_generate_self_attested_proof by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/764
  * Changed Proof (Verifier) API for checking presentation status by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/770
  * Sort error mapping by numeric code by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/771

### Fixes
* OOB invite attachment field conditional serialization, default to empty if not present by @mirgee in https://github.com/hyperledger/aries-vcx/pull/762

### Features
* Expose getting and clearing attributes from the ledger by @mirgee in https://github.com/hyperledger/aries-vcx/pull/767


# uniffi
* UniFFI Proof of Concept by @gmulhearn in https://github.com/hyperledger/aries-vcx/pull/737

# libvcx
* Update nodejs in libvcx docker image to 18.14.2-r0 by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/760
* Split libvcx in 2 crates, update diagrams by @Patrik-Stas in https://github.com/hyperledger/aries-vcx/pull/759

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.53.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-03-22 09:17:52 +0000 UTC
    </span>
</div>

