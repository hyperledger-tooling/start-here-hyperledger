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
                    Release 0.51.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.51.0
                </span>
            </td>
            <td>
                # Changelog

## [0.50.0](https://github.com/hyperledger/aries-vcx/tree/0.50.0) (2022-12-05)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.49.1...0.50.0)

### Other pull requests

- Release 0.50.0 [\#688](https://github.com/hyperledger/aries-vcx/pull/688) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Modularize dependency on vdrtools/indy with option for indy-Vdr and Indy-Credx in place [\#648](https://github.com/hyperledger/aries-vcx/pull/648) ([gmulhearn-anonyome](https://github.com/gmulhearn-anonyome))

## [0.49.1](https://github.com/hyperledger/aries-vcx/tree/0.49.1) (2022-12-04)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.49.0...0.49.1)

### Other pull requests

- Release 0.49.1 [\#687](https://github.com/hyperledger/aries-vcx/pull/687) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Fix legacy wrapper ios release [\#686](https://github.com/hyperledger/aries-vcx/pull/686) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Handle did:sov service omitting routing\_keys attribute [\#676](https://github.com/hyperledger/aries-vcx/pull/676) ([guijd3p](https://github.com/guijd3p))

## [0.49.0](https://github.com/hyperledger/aries-vcx/tree/0.49.0) (2022-12-04)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.48.0...0.49.0)

### Other pull requests

- Add ios legacy wrapper [\#683](https://github.com/hyperledger/aries-vcx/pull/683) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Release 0.49.0 [\#682](https://github.com/hyperledger/aries-vcx/pull/682) ([Patrik-Stas](https://github.com/Patrik-Stas))

## [0.48.0](https://github.com/hyperledger/aries-vcx/tree/0.48.0) (2022-12-02)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.47.0...0.48.0)

### Wrapper changes

- NodeJS wrapper: Update to Node 17 / 18 [\#640](https://github.com/hyperledger/aries-vcx/issues/640)

### Changes to agents

- Implement Storage trait for agent's ObjectCache [\#671](https://github.com/hyperledger/aries-vcx/pull/671) ([mirgee](https://github.com/mirgee))

### Other pull requests

- Release 0.48.0 [\#681](https://github.com/hyperledger/aries-vcx/pull/681) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Align service resolution on indy ledger with did:sov spec [\#672](https://github.com/hyperledger/aries-vcx/pull/672) ([guijd3p](https://github.com/guijd3p))
- Validated some parameters passed as a JSON string. [\#667](https://github.com/hyperledger/aries-vcx/pull/667) ([left-arm](https://github.com/left-arm))
- Do not try to publish libvcx image from fork PRs [\#664](https://github.com/hyperledger/aries-vcx/pull/664) ([Patrik-Stas](https://github.com/Patrik-Stas))
- iOS Wrapper [\#663](https://github.com/hyperledger/aries-vcx/pull/663) ([PaulRps](https://github.com/PaulRps))
- Add other mime type for attributes [\#662](https://github.com/hyperledger/aries-vcx/pull/662) ([pomfar](https://github.com/pomfar))

## [0.47.0](https://github.com/hyperledger/aries-vcx/tree/0.47.0) (2022-11-22)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.46.0...0.47.0)

### Other issues

- Remove the dependency of aries-vcx backchannel on agency [\#651](https://github.com/hyperledger/aries-vcx/issues/651)
- Remove FFI layer to vdr-tools [\#615](https://github.com/hyperledger/aries-vcx/issues/615)

### Other pull requests

- Release 0.47.0 [\#660](https://github.com/hyperledger/aries-vcx/pull/660) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Remove libc as aries-vcx dependency [\#657](https://github.com/hyperledger/aries-vcx/pull/657) ([Patrik-Stas](https://github.com/Patrik-Stas))

## [0.46.0](https://github.com/hyperledger/aries-vcx/tree/0.46.0) (2022-11-21)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.45.0...0.46.0)

### CI changes

- Run nodejs tests with multiple nodejs versions [\#646](https://github.com/hyperledger/aries-vcx/pull/646) ([Patrik-Stas](https://github.com/Patrik-Stas))

### Wrapper changes

- Appending handshake protocols from node wrapper [\#655](https://github.com/hyperledger/aries-vcx/pull/655) ([mirgee](https://github.com/mirgee))
- Update node wrapper dependencies [\#643](https://github.com/hyperledger/aries-vcx/pull/643) ([mirgee](https://github.com/mirgee))
- Expose reading of Aries service from the ledger [\#641](https://github.com/hyperledger/aries-vcx/pull/641) ([mirgee](https://github.com/mirgee))
- Expose key and service creation, message unpacking [\#639](https://github.com/hyperledger/aries-vcx/pull/639) ([mirgee](https://github.com/mirgee))

### Changes to agents

- Replace mediated connection handler with nonmediated connection handler in aries-vcx-agent [\#650](https://github.com/hyperledger/aries-vcx/issues/650)
- Get connection by remote vk, unpack sender vk, remove async, etc. [\#653](https://github.com/hyperledger/aries-vcx/pull/653) ([mirgee](https://github.com/mirgee))

### Refactoring

- Rename connection -\> mediated\_connection in api\_lib [\#658](https://github.com/hyperledger/aries-vcx/pull/658) ([mirgee](https://github.com/mirgee))
- Unify send message closure type, validate connection response on receipt [\#644](https://github.com/hyperledger/aries-vcx/pull/644) ([mirgee](https://github.com/mirgee))

### Other issues

- Process prefixed DIDs in aries messages [\#627](https://github.com/hyperledger/aries-vcx/issues/627)
- Implement support for non-mediated public endpoint [\#618](https://github.com/hyperledger/aries-vcx/issues/618)
- Return presentation status enums instead of u32 code [\#617](https://github.com/hyperledger/aries-vcx/issues/617)
- Implement non-mediated connection handler [\#616](https://github.com/hyperledger/aries-vcx/issues/616)

### Other pull requests

- Release 0.46.0 [\#652](https://github.com/hyperledger/aries-vcx/pull/652) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Add non-mediated connection service to aries-vcx-agent [\#649](https://github.com/hyperledger/aries-vcx/pull/649) ([mirgee](https://github.com/mirgee))
- Non-mediated connection [\#645](https://github.com/hyperledger/aries-vcx/pull/645) ([mirgee](https://github.com/mirgee))
- create prefix did:sov [\#642](https://github.com/hyperledger/aries-vcx/pull/642) ([guijd3p](https://github.com/guijd3p))
- Build and publish libvcx.so [\#629](https://github.com/hyperledger/aries-vcx/pull/629) ([Patrik-Stas](https://github.com/Patrik-Stas))

## [0.45.0](https://github.com/hyperledger/aries-vcx/tree/0.45.0) (2022-11-01)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.44.0...0.45.0)

### CI changes

- Fix test-android-build job dependency [\#637](https://github.com/hyperledger/aries-vcx/pull/637) ([Patrik-Stas](https://github.com/Patrik-Stas))

### Hotfixes

- Fix agent build [\#607](https://github.com/hyperledger/aries-vcx/pull/607) ([mirgee](https://github.com/mirgee))

### Refactoring

- Use Status enums instead of u32 [\#621](https://github.com/hyperledger/aries-vcx/pull/621) ([BulkBeing](https://github.com/BulkBeing))
- Use a macro for message fetching functions in agent [\#612](https://github.com/hyperledger/aries-vcx/pull/612) ([mirgee](https://github.com/mirgee))
- Refactor verifier / prover SMs [\#611](https://github.com/hyperledger/aries-vcx/pull/611) ([mirgee](https://github.com/mirgee))
- Refactor issuer / holder SMs [\#610](https://github.com/hyperledger/aries-vcx/pull/610) ([mirgee](https://github.com/mirgee))
- Backchannel-related refactoring [\#605](https://github.com/hyperledger/aries-vcx/pull/605) ([mirgee](https://github.com/mirgee))

### Other pull requests

- Set up missing MAIN\_BRANCH env variable in CI [\#638](https://github.com/hyperledger/aries-vcx/pull/638) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Revocation status "self-check" [\#635](https://github.com/hyperledger/aries-vcx/pull/635) ([mirgee](https://github.com/mirgee))
- Replace gradlew repo jcenter\(\) by mavenCentral\(\) [\#634](https://github.com/hyperledger/aries-vcx/pull/634) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Cleanup: delete and ignore temporary OS file \(.DS\_Store\) [\#633](https://github.com/hyperledger/aries-vcx/pull/633) ([jodaAtGithub](https://github.com/jodaAtGithub))
- Add .editorconfig [\#632](https://github.com/hyperledger/aries-vcx/pull/632) ([mirgee](https://github.com/mirgee))
- Publish branch image builds in publishing jobs [\#626](https://github.com/hyperledger/aries-vcx/pull/626) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Run tests directly on GA runner [\#622](https://github.com/hyperledger/aries-vcx/pull/622) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Allow obtaining cred rev id from the wallet [\#614](https://github.com/hyperledger/aries-vcx/pull/614) ([mirgee](https://github.com/mirgee))
- Ci/improvements [\#613](https://github.com/hyperledger/aries-vcx/pull/613) ([Patrik-Stas](https://github.com/Patrik-Stas))
- Revocation notification [\#608](https://github.com/hyperledger/aries-vcx/pull/608) ([mirgee](https://github.com/mirgee))
- Rust aries agent [\#604](https://github.com/hyperledger/aries-vcx/pull/604) ([mirgee](https://github.com/mirgee))

## [0.44.0](https://github.com/hyperledger/aries-vcx/tree/0.44.0) (2022-10-07)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.43.0...0.44.0)

## [0.43.0](https://github.com/hyperledger/aries-vcx/tree/0.43.0) (2022-10-06)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.42.0...0.43.0)

## [0.42.0](https://github.com/hyperledger/aries-vcx/tree/0.42.0) (2022-09-20)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.41.0...0.42.0)

## [0.41.0](https://github.com/hyperledger/aries-vcx/tree/0.41.0) (2022-09-05)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.40.0...0.41.0)

## [0.40.0](https://github.com/hyperledger/aries-vcx/tree/0.40.0) (2022-08-24)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.39.0...0.40.0)

## [0.39.0](https://github.com/hyperledger/aries-vcx/tree/0.39.0) (2022-08-04)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.38.0...0.39.0)

## [0.38.0](https://github.com/hyperledger/aries-vcx/tree/0.38.0) (2022-07-28)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.37.0...0.38.0)

## [0.37.0](https://github.com/hyperledger/aries-vcx/tree/0.37.0) (2022-07-01)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.36.0...0.37.0)

## [0.36.0](https://github.com/hyperledger/aries-vcx/tree/0.36.0) (2022-06-07)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.35.0...0.36.0)

## [0.35.0](https://github.com/hyperledger/aries-vcx/tree/0.35.0) (2022-04-13)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.34.0...0.35.0)

## [0.34.0](https://github.com/hyperledger/aries-vcx/tree/0.34.0) (2022-03-22)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.33.0...0.34.0)

## [0.33.0](https://github.com/hyperledger/aries-vcx/tree/0.33.0) (2022-03-02)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.32.0...0.33.0)

## [0.32.0](https://github.com/hyperledger/aries-vcx/tree/0.32.0) (2022-02-25)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.31.0...0.32.0)

## [0.31.0](https://github.com/hyperledger/aries-vcx/tree/0.31.0) (2022-02-10)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.30.0...0.31.0)

## [0.30.0](https://github.com/hyperledger/aries-vcx/tree/0.30.0) (2022-02-08)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.29.0...0.30.0)

## [0.29.0](https://github.com/hyperledger/aries-vcx/tree/0.29.0) (2022-01-26)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.28.0...0.29.0)

## [0.28.0](https://github.com/hyperledger/aries-vcx/tree/0.28.0) (2022-01-12)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.27.0...0.28.0)

## [0.27.0](https://github.com/hyperledger/aries-vcx/tree/0.27.0) (2021-12-17)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.26.0...0.27.0)

## [0.26.0](https://github.com/hyperledger/aries-vcx/tree/0.26.0) (2021-12-09)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.25.0...0.26.0)

## [0.25.0](https://github.com/hyperledger/aries-vcx/tree/0.25.0) (2021-12-06)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.24.2...0.25.0)

## [0.24.2](https://github.com/hyperledger/aries-vcx/tree/0.24.2) (2021-11-30)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.24.1...0.24.2)

## [0.24.1](https://github.com/hyperledger/aries-vcx/tree/0.24.1) (2021-11-25)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.23.0...0.24.1)

## [0.23.0](https://github.com/hyperledger/aries-vcx/tree/0.23.0) (2021-10-27)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.22.0...0.23.0)

## [0.22.0](https://github.com/hyperledger/aries-vcx/tree/0.22.0) (2021-10-21)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.21.0...0.22.0)

## [0.21.0](https://github.com/hyperledger/aries-vcx/tree/0.21.0) (2021-10-05)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.20.2...0.21.0)

## [0.20.2](https://github.com/hyperledger/aries-vcx/tree/0.20.2) (2021-09-01)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.20.1...0.20.2)

## [0.20.1](https://github.com/hyperledger/aries-vcx/tree/0.20.1) (2021-09-01)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.20.0...0.20.1)

## [0.20.0](https://github.com/hyperledger/aries-vcx/tree/0.20.0) (2021-07-19)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.19.0...0.20.0)

## [0.19.0](https://github.com/hyperledger/aries-vcx/tree/0.19.0) (2021-06-28)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.18.3...0.19.0)

## [0.18.3](https://github.com/hyperledger/aries-vcx/tree/0.18.3) (2021-06-16)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.18.2...0.18.3)

## [0.18.2](https://github.com/hyperledger/aries-vcx/tree/0.18.2) (2021-06-09)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.18.1...0.18.2)

## [0.18.1](https://github.com/hyperledger/aries-vcx/tree/0.18.1) (2021-06-03)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.18.0...0.18.1)

## [0.18.0](https://github.com/hyperledger/aries-vcx/tree/0.18.0) (2021-05-31)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.17.3...0.18.0)

## [0.17.3](https://github.com/hyperledger/aries-vcx/tree/0.17.3) (2021-04-30)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.17.2...0.17.3)

## [0.17.2](https://github.com/hyperledger/aries-vcx/tree/0.17.2) (2021-04-27)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.17.1...0.17.2)

## [0.17.1](https://github.com/hyperledger/aries-vcx/tree/0.17.1) (2021-03-29)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.17.0...0.17.1)

## [0.17.0](https://github.com/hyperledger/aries-vcx/tree/0.17.0) (2021-03-24)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.16.0...0.17.0)

## [0.16.0](https://github.com/hyperledger/aries-vcx/tree/0.16.0) (2021-01-21)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.15.0...0.16.0)

## [0.15.0](https://github.com/hyperledger/aries-vcx/tree/0.15.0) (2020-12-22)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.14.2...0.15.0)

## [0.14.2](https://github.com/hyperledger/aries-vcx/tree/0.14.2) (2020-12-04)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.14.0...0.14.2)

## [0.14.0](https://github.com/hyperledger/aries-vcx/tree/0.14.0) (2020-11-26)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.13.1...0.14.0)

## [0.13.1](https://github.com/hyperledger/aries-vcx/tree/0.13.1) (2020-11-10)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.13.0...0.13.1)

## [0.13.0](https://github.com/hyperledger/aries-vcx/tree/0.13.0) (2020-11-10)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.12.0...0.13.0)

## [0.12.0](https://github.com/hyperledger/aries-vcx/tree/0.12.0) (2020-10-27)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.11.0...0.12.0)

## [0.11.0](https://github.com/hyperledger/aries-vcx/tree/0.11.0) (2020-10-02)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.10.0...0.11.0)

## [0.10.0](https://github.com/hyperledger/aries-vcx/tree/0.10.0) (2020-09-24)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.9.1...0.10.0)

## [0.9.1](https://github.com/hyperledger/aries-vcx/tree/0.9.1) (2020-08-25)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/0.8.0...0.9.1)

## [0.8.0](https://github.com/hyperledger/aries-vcx/tree/0.8.0) (2020-03-31)

[Full Changelog](https://github.com/hyperledger/aries-vcx/compare/d48fe2d71a839a873113890d9808c531da643288...0.8.0)




            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-vcx/releases/tag/0.51.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-01-09 16:55:09 +0000 UTC
    </span>
</div>

