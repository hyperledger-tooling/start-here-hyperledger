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
                    0.10.2-rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.10.2-rc0
                </span>
            </td>
            <td>
                Release 0.10.2 is a patch release for 0.10.1 that addresses two specific regressions found
in deploying Release 0.10.1. The regressions are to fix:

- An ACA-Py instance upgraded to 0.10.1 that had an existing connection to another Aries agent
where the connection has both an `http` and `ws` (websocket) service endpoint with the same ID cannot
message that agent. A scenario is an ACA-Py issuer connecting to an Endorser with both `http` and
`ws` service endpoints. The updates made in 0.10.1 to improve ACA-Py DID resolution did not account
for this scenario and needed a tweak to work ([Issue \#2474], [PR \#2475]).
- The "fix revocation registry" endpoint used to fix scenarios an Issuer's local revocation registry
state is out of sync with the ledger was broken by some code being added to support a single
ACA-Py instance writing to different ledgers ([Issue \#2477], [PR \#2480]).

[Issue \#2474]: https://github.com/hyperledger/aries-cloudagent-python/issue/2474
[PR \#2475]: https://github.com/hyperledger/aries-cloudagent-python/pull/2476
[Issue \#2477]: https://github.com/hyperledger/aries-cloudagent-python/issue/2477
[PR \#2480]: https://github.com/hyperledger/aries-cloudagent-python/pull/2480

## What's Changed
* 0.10.2 Patch Release - fix issue #2475, #2477 by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2482
* 0.10.2 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2484


**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.10.1...0.10.2-rc0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.10.2-rc0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-09-08 02:34:07 +0000 UTC
    </span>
</div>

