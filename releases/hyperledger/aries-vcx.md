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
                    Release 0.45.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.45.0
                </span>
            </td>
            <td>
                # Changelog

## [0.45.0](https://github.com/hyperledger/aries-vcx/tree/0.45.0) (2022-11-01)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.44.0...0.45.0)

### Features
- Rust aries-vcx agent https://github.com/hyperledger/aries-vcx/pull/604
- Add API to get crev_rev_id https://github.com/hyperledger/aries-vcx/pull/614
- Implement revocation notification (Aries RFC 0183) https://github.com/hyperledger/aries-vcx/pull/608
- Implement API to enable issuer/holder to verify against ledger whether a credential is revoked https://github.com/hyperledger/aries-vcx/pull/635

### Cleanups / refactoring
- Stripped down vdr-tools dependencies https://github.com/hyperledger/aries-vcx/pull/596
- Removed unused imports https://github.com/hyperledger/aries-vcx/pull/595
- Refactoring of cred-defs / schemas https://github.com/hyperledger/aries-vcx/pull/605
- Issuer/Holder state machines refactoring https://github.com/hyperledger/aries-vcx/pull/610
- Prover/Verifier state machines refactoring https://github.com/hyperledger/aries-vcx/pull/611
- Refactor return values from state machines https://github.com/hyperledger/aries-vcx/pull/621

### Breaking changes
- Require initialization of runtime https://github.com/hyperledger/aries-vcx/pull/598

### Other issues
- Prevent double initialization of logger https://github.com/hyperledger/aries-vcx/pull/599

### CI
- Reuse CI code using composite actions https://github.com/hyperledger/aries-vcx/pull/603
- Update rust toolchain to 1.64 https://github.com/hyperledger/aries-vcx/pull/602
- Rework CI to run on GA runners instead of docker https://github.com/hyperledger/aries-vcx/pull/613




            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.45.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-11-01 13:26:14 +0000 UTC
    </span>
</div>

