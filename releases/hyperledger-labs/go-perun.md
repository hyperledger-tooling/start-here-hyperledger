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
                    Ganymede
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.7.0
                </span>
            </td>
            <td>
                Virtual channels. And some other additions.

### Added :sparkles:
- **Virtual Channels** ([#83](https://github.com/hyperledger-labs/go-perun/pull/83), [#114](https://github.com/hyperledger-labs/go-perun/pull/114), [#119](https://github.com/hyperledger-labs/go-perun/pull/119), [#123](https://github.com/hyperledger-labs/go-perun/pull/123)): Go-perun now supports virtual channels. A virtual channel is a channel that is funded and settled completely off-chain and therefore does not incur any on-chain transaction fees.
- **Generic event subscription** ([#36](https://github.com/hyperledger-labs/go-perun/pull/36), [#86](https://github.com/hyperledger-labs/go-perun/pull/86), [#89](https://github.com/hyperledger-labs/go-perun/pull/89), [#94](https://github.com/hyperledger-labs/go-perun/pull/94)): In preparation for implementing a reorg-resistant event subscription, we implemented a generic event subscription that can be used across the whole library.
- **Tutorial announcement** ([c8cff7cb](https://github.com/perun-network/go-perun/commit/c8cff7cbbe97e5b2127e7109483026d1b3938453)): We now have a developer tutorial at [http://tutorial.perun.network](http://tutorial.perun.network).
- **Named errors** ([429a8934](https://github.com/perun-network/go-perun/commit/429a8934666db35d99186d874c23f1102e78750d), [#10](https://github.com/hyperledger-labs/go-perun/pull/10), [#11](https://github.com/hyperledger-labs/go-perun/pull/11), [#26](https://github.com/hyperledger-labs/go-perun/pull/26), [#34](https://github.com/hyperledger-labs/go-perun/pull/34), [#80](https://github.com/hyperledger-labs/go-perun/pull/80)): Specific error types help the library user to identify the cause of an error.
- **Register asset at runtime** [#124](https://github.com/hyperledger-labs/go-perun/pull/124): It is now possible to add assets to the Eth funder at runtime.
- `Gatherer.OnFail` ([e3729a6a](https://github.com/perun-network/go-perun/commit/e3729a6a2f0231273d1cb4ee05ef113c335cdb05)),
Test wallet ([12c78d33](https://github.com/perun-network/go-perun/commit/12c78d33ba339a328d8e5a7b7cf241d9cafca157)),
GitHub CI ([#3](https://github.com/hyperledger-labs/go-perun/pull/3)),
`ConcurrentT.WaitCtx` ([#112](https://github.com/hyperledger-labs/go-perun/pull/112)),
Eth sim backend auto mining ([#104](https://github.com/hyperledger-labs/go-perun/pull/104))

### Changed :construction:
- [:boom:] **Asset holder validation** ([#111](https://github.com/hyperledger-labs/go-perun/pull/111)): Asset holder validation does no longer include adjudicator validation.
- **Current state in HandleUpdate** [#33](https://github.com/hyperledger-labs/go-perun/pull/33): The update handler now receives the current channel state as a parameter.
- **Funder usability** [#74](https://github.com/hyperledger-labs/go-perun/pull/74): Streamlined Eth funder setup.
- 2021 updates ([2212847d](https://github.com/perun-network/go-perun/commit/2212847de68d683865427c7e11abd48b589f90ee)),
Update generate script ([3f81e47c](https://github.com/perun-network/go-perun/commit/3f81e47cfe436ec42ed4ae9d91742e58f64a0013)),
Update links to HLL ([#6](https://github.com/hyperledger-labs/go-perun/pull/6)),
Update security disclaimer ([#14](https://github.com/hyperledger-labs/go-perun/pull/14), [#51](https://github.com/hyperledger-labs/go-perun/pull/51)),
Delete gitlab templates ([#24](https://github.com/hyperledger-labs/go-perun/pull/24)),
Dependency update ([#30](https://github.com/hyperledger-labs/go-perun/pull/30)),
Document parameters of `NewLedgerChannelProposal` ([#43](https://github.com/hyperledger-labs/go-perun/pull/43)),
CI speed-up ([#44](https://github.com/hyperledger-labs/go-perun/pull/44)),
Refactor Eth channel errors ([#88](https://github.com/hyperledger-labs/go-perun/pull/88)),
Log message type ([#96](https://github.com/hyperledger-labs/go-perun/pull/96))

### Fixed :bug:
- **Cache first channel update** ([#4](https://github.com/hyperledger-labs/go-perun/pull/4), [#129](https://github.com/hyperledger-labs/go-perun/pull/129)): Fixes a bug where a client receives channel messages before completing the channel setup.
- **Subchannel off-chain settlement** [#59](https://github.com/hyperledger-labs/go-perun/pull/59): Sub-channels had to be disputed on-chain before they could be settled. Sub-channels can now be collaboratively settled off-chain.
- **ERC20 depositor nonce mismatch** [#134](https://github.com/hyperledger-labs/go-perun/pull/134): Fixes an issue where the ERC20 depositor sometimes was not incrementing the transaction nonce correctly.

- Unitialized funder variable ([af207adb](https://github.com/perun-network/go-perun/commit/af207adb385329f2b5c0af0fff90c495639a7bf5)),
EndpointRegistry retry and timeout ([28e535bb](https://github.com/perun-network/go-perun/commit/28e535bb6302959c321876968bf1083473824675)),
Watcher return ([cf9279c9](https://github.com/perun-network/go-perun/commit/cf9279c99f73db1f665c072edcd82167888fe83f)),
Thread-safe test wallet [#17](https://github.com/hyperledger-labs/go-perun/pull/17),
Withdraw variable capture [#50](https://github.com/hyperledger-labs/go-perun/pull/50),
`NewRandomLedgerChannelProposal` consistency [#55](https://github.com/hyperledger-labs/go-perun/pull/55),
Enable logging per default in package client [#66](https://github.com/hyperledger-labs/go-perun/pull/66),
Stabilize `BlockTimeout` test [#90](https://github.com/hyperledger-labs/go-perun/pull/90),
Fix state hash test [#120](https://github.com/hyperledger-labs/go-perun/pull/120),
Ensure custom error progagation [#126](https://github.com/hyperledger-labs/go-perun/pull/126)

### Security :lock:
- **Ensure correct params ID after deserialization** [#60](https://github.com/hyperledger-labs/go-perun/pull/60): Parameter deserialization did not assert that the encoded channel ID is correct. This is now fixed.
- **Signature verification for sub-channel funding and settlement** [#61](https://github.com/hyperledger-labs/go-perun/pull/61): Sub-channel funding and settlement requires an automated update in the parent channel. The signatures on that automated update were not correctly verified. This is now fixed.
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/go-perun/releases/tag/v0.7.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-07-14 16:00:28 +0000 UTC
    </span>
</div>

