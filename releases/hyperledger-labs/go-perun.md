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
                    Io
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.9.0
                </span>
            </td>
            <td>
                Injectable wire encoding and a `protobuf` wire encoder.

### Added

- :sparkles: **Injectable wire encoding [#233]:** The encoding used for messages that are sent across the network is now injectable.
  - Add binary marshalling: [#272], [#284], [#298].
  - Add serializer interface: [#297], [#325].
  - Change the mechanism for generating `ProposalID`: [#300], [#307].
  - Rename message types [#305].
  - Extend and refactor message serialization tests: [#316], [#317].
- :sparkles: **Protobuf wire encoder [#311]:** A wire encoder based on `protobuf` has been added [#318].
- Minor additions: Introduce `Asset.Equal` [#279], export proposer index [#313].

### Changed

- :boom: Rename `Address.Equals` to `Address.Equal` [#264].
- :boom: Revise `Channel.Update` and `Channel.ForceUpdate`: [#289], [#291], [#306].
- :truck: `pkg/io` migration: [#256], [#271], [#285], [#287].
- :memo: Update README to include references to existing backends [#314].
- :children_crossing: Minor usability improvements: [#268], [#278], [#315].
- :construction_worker: CI updates: [#260], [#274], [#276], [#277].
- :arrow_up: Use `LatestSigner` in Ethereum contract backend and don't set `GasLimit` by default, so that [EIP1559](https://eips.ethereum.org/EIPS/eip-1559) TXs are sent [#322].

### Fixed
- :bug: Fix a bug causing `Channel.Watch` to not work correctly for sub-channels and virtual channels [#251].
- :bug: Fix bugs causing `ContractBackend.confirmNTimes` to block indefintely or fail in some rare cases: [#254], [#309].
- :white_check_mark: Improve test stability: [#310], [#319].

### Security
- :lock: It is now checked that assets are not changed during a state update, which could otherwise cause a channel to become unfunded [#304].

[#233]: https://github.com/hyperledger-labs/go-perun/issues/233
[#311]: https://github.com/hyperledger-labs/go-perun/issues/311

[#251]: https://github.com/hyperledger-labs/go-perun/pull/251
[#254]: https://github.com/hyperledger-labs/go-perun/pull/254
[#256]: https://github.com/hyperledger-labs/go-perun/pull/256
[#260]: https://github.com/hyperledger-labs/go-perun/pull/260
[#264]: https://github.com/hyperledger-labs/go-perun/pull/264
[#268]: https://github.com/hyperledger-labs/go-perun/pull/268
[#271]: https://github.com/hyperledger-labs/go-perun/pull/271
[#272]: https://github.com/hyperledger-labs/go-perun/pull/272
[#274]: https://github.com/hyperledger-labs/go-perun/pull/274
[#276]: https://github.com/hyperledger-labs/go-perun/pull/276
[#277]: https://github.com/hyperledger-labs/go-perun/pull/277
[#278]: https://github.com/hyperledger-labs/go-perun/pull/278
[#279]: https://github.com/hyperledger-labs/go-perun/pull/279
[#284]: https://github.com/hyperledger-labs/go-perun/pull/284
[#285]: https://github.com/hyperledger-labs/go-perun/pull/285
[#287]: https://github.com/hyperledger-labs/go-perun/pull/287
[#289]: https://github.com/hyperledger-labs/go-perun/pull/289
[#291]: https://github.com/hyperledger-labs/go-perun/pull/291
[#297]: https://github.com/hyperledger-labs/go-perun/pull/297
[#298]: https://github.com/hyperledger-labs/go-perun/pull/298
[#300]: https://github.com/hyperledger-labs/go-perun/pull/300
[#304]: https://github.com/hyperledger-labs/go-perun/pull/304
[#305]: https://github.com/hyperledger-labs/go-perun/pull/305
[#306]: https://github.com/hyperledger-labs/go-perun/pull/306
[#307]: https://github.com/hyperledger-labs/go-perun/pull/307
[#309]: https://github.com/hyperledger-labs/go-perun/pull/309
[#310]: https://github.com/hyperledger-labs/go-perun/pull/310
[#313]: https://github.com/hyperledger-labs/go-perun/pull/313
[#314]: https://github.com/hyperledger-labs/go-perun/pull/314
[#315]: https://github.com/hyperledger-labs/go-perun/pull/315
[#316]: https://github.com/hyperledger-labs/go-perun/pull/316
[#317]: https://github.com/hyperledger-labs/go-perun/pull/317
[#318]: https://github.com/hyperledger-labs/go-perun/pull/318
[#319]: https://github.com/hyperledger-labs/go-perun/pull/319
[#322]: https://github.com/hyperledger-labs/go-perun/pull/322
[#325]: https://github.com/hyperledger-labs/go-perun/pull/325
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/go-perun/releases/tag/v0.9.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-02-25 14:31:37 +0000 UTC
    </span>
</div>

