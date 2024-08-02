---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.12.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.12.2
                </span>
            </td>
            <td>
                A patch release to add the verification of a linkage between an inbound message and its associated connection (if any) before processing the message. Also adds some additional cleanup/fix PRs from the main branch (see list below) that might be useful for deployments currently using [Release 0.12.1](#0121) or [0.12.0](#0120).

### 0.12.2 Breaking Changes

There are no breaking changes in this release.

### PRs cherry-picked from the `main` branch:
  - fix: multiuse invites with did peer 4 [\#3112](https://github.com/hyperledger/aries-cloudagent-python/pull/3112) [dbluhm](https://github.com/dbluhm)
  - Check connection is ready in all connection required handlers [\#3095](https://github.com/hyperledger/aries-cloudagent-python/pull/3095) [jamshale](https://github.com/jamshale)
  - Add by_format to terse webhook for presentations [\#3081](https://github.com/hyperledger/aries-cloudagent-python/pull/3081) [ianco](https://github.com/ianco)
  - fix: respond to did:peer:1 with did:peer:4 [\#3050](https://github.com/hyperledger/aries-cloudagent-python/pull/3050) [dbluhm](https://github.com/dbluhm)
  - feat: soft binding for plugin flexibility [\#3010](https://github.com/hyperledger/aries-cloudagent-python/pull/3010) [dbluhm](https://github.com/dbluhm)
  - feat: inject profile and session [\#2997](https://github.com/hyperledger/aries-cloudagent-python/pull/2997) [dbluhm](https://github.com/dbluhm)
  - feat: external signature suite provider interface [\#2835](https://github.com/hyperledger/aries-cloudagent-python/pull/2835) [dbluhm](https://github.com/dbluhm)
  - fix(interop): overly strict validation [\#2943](https://github.com/hyperledger/aries-cloudagent-python/pull/2943) [dbluhm](https://github.com/dbluhm)


## What's Changed
* Patch release 0.12.x by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3121
* 0.12.2rc1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/3123
* [ PATCH ] 0.12.x with PR 3081 terse webhooks by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3141
* 0.12.2 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/3145


**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.12.1...0.12.2
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.12.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-08-01 22:21:40 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.11.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.11.3
                </span>
            </td>
            <td>
                A patch release to add a fix that ensures that sufficient webhook information is sent to an ACA-Py controller that is executing the [AIP 2.0 Present Proof 2.0 Protocol].

[AIP 2.0 Present Proof 2.0 Protocol]: https://hyperledger.github.io/aries-rfcs/latest/aip2/0454-present-proof-v2/

### 0.11.3 Breaking Changes

There are no breaking changes in this release.

### 0.11.3 PRs Cherry-picked from the `main` branch

- Add by_format to terse webhook for presentations [\#3081](https://github.com/hyperledger/aries-cloudagent-python/pull/3081) [ianco](https://github.com/ianco)

## What's Changed
* [ PATCH ] 0.11.x with PR 3081 terse webhooks by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3142
* 0.11.3 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/3144


**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.11.2...0.11.3
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.11.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-08-01 22:16:46 +0000 UTC
    </span>
</div>

