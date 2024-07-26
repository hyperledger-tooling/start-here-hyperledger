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
                    2.0.0-pre-rc.22.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.0.0-pre-rc.22.0
                </span>
            </td>
            <td>
                ### Added

- specify on-chain parameters explicitly in genesis (#4812)
- allow turbofish with multiple `Instruction`s (#4805)
- reimplement multisignature transactions (#4788)
- implement built-in vs custom on-chain parameters (#4731)
- improve custom instruction usage (#4778)
- make the metadata dynamic via implementing JsonString (#4732)
- allow multiple peers submit genesis block (#4775)
- supply `SignedBlock` instead of `SignedTransaction` to peer (#4739)
- custom instructions in executor (#4645)
- extend client cli to request json queries (#4684)
- add detect support for `parity_scale_decoder` (#4680)
- generalize permissions schema to executor data model (#4658)
- added register trigger permissions in the default executor (#4616)
- support JSON in `parity_scale_cli`
- deduplicate triggers with the same wasm code (#4434)
- introduce p2p idle timeout

### Changed

- replace `lol_alloc` with `dlmalloc` (#4857)
- rename `type_` to `type` in schema (#4855)
- replace `Duration` with `u64` in schema (#4841)
- use `RUST_LOG`-like EnvFilter for logging (#4837)
- keep voting block when possible (#4828)
- migrate from warp to axum (#4718)
- split executor data model (#4791)
- shallow data model (#4734) (#4792)
- don't send public key with signature (#4518)
- rename `--outfile` to `--out-file` (#4679)
- rename iroha server and client (#4662)
- rename `PermissionToken` to `Permission` (#4635)
- reject `BlockMessages` eagerly (#4606)
- make `SignedBlock` immutable (#4620)
- rename TransactionValue into CommittedTransaction (#4610)
- authenticate personal accounts by ID (#4411)
- use multihash format for private keys (#4541)
- rename `parity_scale_decoder` to `parity_scale_cli`
- send blocks to observing peers
- make `Role` transparent (#4886)
- derive block hash from header (#4890)

### Fixed

- check that authority owns domain to transfer (#4807)
- remove logger double initialization (#4800)
- fix naming convention for assets and permissions (#4741)
- upgrade executor in separate transaction in genesis block (#4757)
- make `iroha_smart_contract_utils` `log` and `dbg` functions work outside of wasm (#4725)
- correct default value for `JsonString` (#4692)
- improve deserialization error message (#4659)
- do not panic if the passed Ed25519Sha512 public key is of invalid length (#4650)
- use proper view change index on init block load (#4612)
- don't prematurely execute time-triggers before their `start` timestamp (#4333)
- support `https` for `torii_url` (#4601) (#4617)
- remove serde(flatten) from SetKeyValue/RemoveKeyValue (#4547)
- trigger set is correctly serialized
- revoke removed `PermissionToken`s on `Upgrade<Executor>` (#4503)
- report correct view change index for current round
- remove corresponding triggers on `Unregister<Domain>` (#4461)
- check genesis pub key in genesis round
- prevent registering genesis Domain or Account
- remove permissions from roles on entity unregistration
- trigger metadata is accessible in smart contracts
- use rw lock to prevent inconsitent state view (#4867)
- handle soft fork in snapshot (#4868)
- fix MinSize for ChaCha20Poly1305
- add limits to LiveQueryStore to prevent high memory usage (#4893)

### Removed

- remove public key from ed25519 private key (#4856)
- remove kura.lock (#4849)
- revert `_ms` and `_bytes` suffixes in config (#4667)
- remove `_id` and `_file` suffix from genesis fields (#4724)
- remove index Assets in AssetsMap by AssetDefinitionId (#4701)
- remove domain from trigger identity (#4640)
- remove genesis signing from Iroha (#4673)
- remove `Visit` bound from `Validate` (#4642)
- remove `TriggeringEventFilterBox` (#4866)
- remove `garbage` in p2p handshake (#4889)
- remove `committed_topology` from block (#4880)

### Security

- sign all query parameters, implement query filters in wasm
- guard against secrets leakage
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/iroha/releases/tag/v2.0.0-pre-rc.22.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-26 09:10:23 +0000 UTC
    </span>
</div>

