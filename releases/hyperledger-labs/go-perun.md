---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Kiviuq
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.11.0
                </span>
            </td>
            <td>
                Exposure of protobuf converters & `SignedState`, abstraction of tests and bug fixes.

## Added
- Add Fabric to backend list in README: [#377]
- Create new type `TransparentChannel` to expose `SignedState`: [#389]
- Update backend compatibility list in README: [#392]
- Add MAINTAINERS.md file, Update NOTICE: [#394]

## Fixed 
- Fix sub-channel test: [#359]
- Fix Multi-Adjudicator Subscription: [#366]
- Use correct identity for client tests: [#376]
- Fix link to white paper in README: [#379]
- Fix linter copyright year checking in CI: [#389]
- Fix failing unit tests: [#399]

## Changed :boom:
- Abstract multiledger test, making it usable by backends: [#355]
- Abstract fund recovery test, making it usable by backends: [#370]
- Abstract virtual channel test, making it usable by backends: [#375]
- Expose protobuf converters: [#384] [#393]
- Use absolute module path in wire.proto: [#383]
- Create AppID Type to generalize app identifiers: [#378] :boom:


[#359]: https://github.com/hyperledger-labs/go-perun/pull/359
[#355]: https://github.com/hyperledger-labs/go-perun/pull/355
[#366]: https://github.com/hyperledger-labs/go-perun/pull/366
[#370]: https://github.com/hyperledger-labs/go-perun/pull/370
[#375]: https://github.com/hyperledger-labs/go-perun/pull/375
[#376]: https://github.com/hyperledger-labs/go-perun/pull/376
[#377]: https://github.com/hyperledger-labs/go-perun/pull/377
[#378]: https://github.com/hyperledger-labs/go-perun/pull/378
[#379]: https://github.com/hyperledger-labs/go-perun/pull/379
[#383]: https://github.com/hyperledger-labs/go-perun/pull/383
[#384]: https://github.com/hyperledger-labs/go-perun/pull/384
[#389]: https://github.com/hyperledger-labs/go-perun/pull/389
[#392]: https://github.com/hyperledger-labs/go-perun/pull/392
[#393]: https://github.com/hyperledger-labs/go-perun/pull/393
[#394]: https://github.com/hyperledger-labs/go-perun/pull/394
[#399]: https://github.com/hyperledger-labs/go-perun/pull/399

## Legend
- <span id="breaking">:boom:</span> This is a breaking change, e.g., it changes the external API.

[:boom:]: #breaking
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/go-perun/releases/tag/v0.11.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-02-20 15:34:30 +0000 UTC
    </span>
</div>

