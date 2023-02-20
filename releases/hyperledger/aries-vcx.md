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
                    Release 0.52.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.52.0
                </span>
            </td>
            <td>
                # Changelog

## [0.52.0](https://github.com/hyperledger/aries-vcx/tree/0.52.0) (2023-02-19)

# aries-vcx

### Typestate connections
- Rewrote `Connection` using Rust typestate pattern in https://github.com/hyperledger/aries-vcx/pull/739
- Additional adjustments in succession: https://github.com/hyperledger/aries-vcx/pull/752, https://github.com/hyperledger/aries-vcx/pull/749

### Refactoring
- Embedded vdr-tools dependency in the repo https://github.com/hyperledger/aries-vcx/pull/732
- Removed unnecessary code from vdr-tools https://github.com/hyperledger/aries-vcx/pull/736

### Dependencies
- Updated `tokio` to `1.20.4` https://github.com/hyperledger/aries-vcx/pull/744

# libvcx
### iOS libvcx wrapper
- Fix `credentialGetOffers` signature https://github.com/hyperledger/aries-vcx/pull/748

### NoteJS wrapper
- Expose function to write `service` attribute on ledger according to `did:sov` method https://github.com/hyperledger/aries-vcx/pull/756

### CI
- Fixes to NodeJS testing CI https://github.com/hyperledger/aries-vcx/pull/750


[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.51.1...0.52.0)




            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.52.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-02-19 22:16:49 +0000 UTC
    </span>
</div>

