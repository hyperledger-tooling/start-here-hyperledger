---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    2.0.0-pre-rc.21
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.0.0-pre-rc.21
                </span>
            </td>
            <td>
                ### Added

- include trigger id in trigger entrypoint (#4391)
- expose event set as bitfields in schema (#4381)
- introduce new `wsv` with granular access (#2664)
- add event filters for `PermissionTokenSchemaUpdate`, `Configuration` and `Executor` events
- introduce snapshot "mode" (#4365)
- allow granting/revoking role's permissions (#4244)
- introduce arbitrary-precision numeric type for assets (remove all other numeric types) (#3660)
- different fuel limit for Executor (#3354)
- integrate pprof profiler (#4250)
- add asset subcommand in client CLI (#4200)
- `Register<AssetDefinition>` permissions (#4049)
- add `chain_id` to prevent replay attacks (#4185)
- add subcommands to edit domain metadata in client CLI (#4175)
- implement store set, remove, get operations in Client CLI (#4163)
- count identical smart contracts for triggers (#4133)
- add subcommand into client CLI to transfer domains (#3974)
- support boxed slices in FFI (#4062)
- git commit SHA to client CLI (#4042)
- proc macro for default validator boilerplate (#3856)
- build progress information to `wasm_builder_cli` (#3237)
- introduced query request builder into Client API (#3124)
- lazy queries inside smart contracts (#3929)
- `fetch_size` query parameter (#3900)
- asset store tranfer instruction (#4258)
- guard against secrets leakage (#3240)
- deduplicate triggers with the same source code (#4419)

### Changed

- bump rust toolchain to nightly-2024-04-18
- send blocks to observing peers (#4387)
- split pipeline events into block and transaction events (#4366)
- rename `[telemetry.dev]` config section to `[dev_telemetry]` (#4377)
- make `Action` and `Filter` non-generic types (#4375)
- improve event filtering API with builder pattern (#3068)
- unify various event filter APIs, introduce a fluent builder API
- rename `FilterBox` into `EventFilterBox`
- rename `TriggeringFilterBox` into `TriggeringEventFilterBox`
- improve filter naming, e.g. `AccountFilter` -> `AccountEventFilter`
- rewrite config according to the configuration RFC (#4239)
- hide internal structure of the versioned structs from the public API (#3887)
- temporarily introduce predictable ordering after too many failed view changes (#4263)
- use concrete key types in `iroha_crypto` (#4181)
- split view changes from normal messages (#4115)
- make `SignedTransaction` immutable (#4162)
- export `iroha_config` through `iroha_client` (#4147)
- export `iroha_crypto` through `iroha_client` (#4149)
- export `data_model` through `iroha_client` (#4081)
- remove `openssl-sys` dependency from `iroha_crypto` and introduce configurable tls backends to `iroha_client` (#3422)
- replace unmaintained EOF `hyperledger/ursa` with in-house solution `iroha_crypto` (#3422)
- optimize executor performance (#4013)
- topology peer update (#3995)

### Fixed

- remove corresponding triggers on `Unregister<Domain>` (#4461)
- remove permissions from roles on entity unregistration (#4242)
- assert that genesis tranasction is signed by genesis pub key (#4253)
- introduce timeout for unresponsive peers in p2p (#4267)
- prevent registering genesis Domain or Account (#4226)
- `MinSize` for `ChaCha20Poly1305` (#4395)
- start console when `tokio-console` is enabled (#4377)
- separate each item with `\n` and recursively create parent directories for `dev-telemetry` file logs
- prevent account registration without signatures (#4212)
- key pair generation is now infallible (#4283)
- stop encoding `X25519` keys as `Ed25519` (#4174)
- do signature validation in `no_std` (#4270)
- calling blocking methods within async context (#4211)
- revoke associated tokens on entity unregistretration (#3962)
- async blocking bug when starting Sumeragi
- fixed `(get|set)_config` 401 HTTP (#4177)
- `musl` archiver name in Docker (#4193)
- smart contract debug print (#4178)
- topology update on restart (#4164)
- registration of new peer (#4142)
- on-chain predictable iteration order (#4130)
- re-architect logger and dynamic configuration (#4100)
- trigger atomicity (#4106)
- query store message ordering issue (#4057)
- set `Content-Type: application/x-parity-scale` for endpoints which reply using SCALE

### Removed

- `logger.tokio_console_address` configuration parameter (#4377)
- `NotificationEvent` (#4377)
- `Value` enum (#4305)
- MST aggregation from iroha (#4229)
- cloning for ISI and query execution in smart contracts (#4182)
- `bridge` and `dex` features (#4152)
- flattened events (#3068)
- expressions (#4089)
- auto-generated config reference
- `IROHA_SKIP_WASM_CHECKS` env variable (#4096)
- `warp` noise in logs (#4097)

### Security

- prevent pub key spoofing in p2p (#4065)
- ensure the `secp256k1` signatures coming out of OpenSSL are normalized (#4155)

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/iroha/releases/tag/v2.0.0-pre-rc.21" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-04-19 10:58:34 +0000 UTC
    </span>
</div>

