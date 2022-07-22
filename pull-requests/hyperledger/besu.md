---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4152" class=".btn">#4152</a>
            </td>
            <td>
                <b>
                    Feature/test peers poc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 13:37:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4150" class=".btn">#4150</a>
            </td>
            <td>
                <b>
                    fix 1 byte long disconnect reason
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixing https://github.com/hyperledger/besu/issues/4071

Signed-off-by: Stefan <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 09:18:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4149" class=".btn">#4149</a>
            </td>
            <td>
                <b>
                    Reduce RocksDB space amplification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reduce RocksDB space amplification with level_compaction_dynamic_level_bytes option set to true. In this case, the size target of levels is changed dynamically based on the size of the last level.

Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 15:27:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4148" class=".btn">#4148</a>
            </td>
            <td>
                <b>
                    add enr peers to discovery layer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 11:52:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4146" class=".btn">#4146</a>
            </td>
            <td>
                <b>
                    API Method: rollup_createPayload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Adds a new api method `rollup_createPayloadV1` as an extension to [Engine API](https://github.com/ethereum/execution-apis/blob/main/src/engine/specification.md) in order to allow to use Besu a L2 execution engine for Rollups;

This method allows to create a Payload with a given list of transactions, executed by it's given order. Invalid transactions are returned with error reason. Unprocessed transactions that don't fit within block gasLimit are returned as well.

To enable this method and rollup behaviour, Besu should run with `--engine-rollup-extension-enabled=true` on CLI

#### Request
Arguments:
- `parentBlockHash`: DATA, 32 Bytes - hash of parent block of this new payload;
- `transactions`:  Array of DATA - Array of transaction objects, each object is a byte list (DATA) representing TransactionType || TransactionPayload or LegacyTransaction as defined in [EIP-2718](https://eips.ethereum.org/EIPS/eip-2718)
- `prevRandao`: DATA, 32 Bytes - value for the prevRandao field of the new payload
- `feeRecipient`: DATA, 20 Bytes - suggested value for the feeRecipient field of the new payload
- `timestamp`: QUANTITY, 64 Bits - value for the timestamp field of the new payload

```json
{
    "id": "100",
    "jsonrpc": "2.0",
    "method": "rollup_createPayloadV1",
    "params": [
        "0xa326af38b7ad1ba192c00b89675c450ffd8e30d83c128ef37a62da26b9f58b9d",
        [
            "0xf86180820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8026a0b7b0cc34f06e99da2a0eb3f290be06fa5982e5b7883b9d2a46e09ee03861955ba008972a7505395050eb78e332d811049c824534a46d751b8305e1b3f819533017",
            "0xf8610a820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8025a09f0f2f41a2a7228d342b81f3937441a0767e5d78c25c86a8e5e5bec7e5fd3b33a02775ee8f94d673774f7f6fd090fa4ccd15b797a47236d59c0ad83549191660e4",
            "0xf86a01820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f96890ad78ebc5ac62000008025a0f6aee06079ff380ec5f0ef90f291b10450636698e9a8bf00484cb06d33713eaba01432b9e6739dcd50d4fbb0555be8a10c7aefb77364816b4493acbc608022deaf",
            "0xf86301820bb88405f5e10094f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8025a072d6b19aba780fdeb57fab5302bf142c5216f45c845267dca77f9d3e20910d44a05390bc4260c188e55a571f1d6a06ff9168391d4c8a7a498a2db49e41063f4b77",
            "0xf86101820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960c8026a096f3751f75a5eeb8f2e27167619ae24efcbb26cf1f5ee6d501ace868398c27dca0740ebd0912eae820d99083c671cf6a483b229a06e28d5e7a215b617cad24f28f",
            "0xf86180820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8026a0b7b0cc34f06e99da2a0eb3f290be06fa5982e5b7883b9d2a46e09ee03861955ba008972a7505395050eb78e332d811049c824534a46d751b8305e1b3f819533017"
        ],
        "0x284ae7412fa90216034852e4ecf953e69df541d323eb8c826442d7b71e5727f6",
        "0xcefc6c8fde4967c755e0e10144914e6d5571b088",
        "0x62d92263"
    ]
}
```

#### Response
```json
{
  "jsonrpc" : "2.0",
  "id" : "100",
  "result" : {
    "status" : "PROCESSED",
    "payloadId" : "0x000000002c94e08a",
    "executionPayload" : {
      "parentHash" : "0xa326af38b7ad1ba192c00b89675c450ffd8e30d83c128ef37a62da26b9f58b9d",
      "feeRecipient" : "0xcefc6c8fde4967c755e0e10144914e6d5571b088",
      "stateRoot" : "0xbce737f398b50b7675f36498184deff0ed134097890fc1ed8ebc2126d49a5ef5",
      "receiptsRoot" : "0xd95b673818fa493deec414e01e610d97ee287c9421c8eff4102b1647c1a184e4",
      "logsBloom" : "0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000",
      "prevRandao" : "0x284ae7412fa90216034852e4ecf953e69df541d323eb8c826442d7b71e5727f6",
      "blockNumber" : "0x1",
      "gasLimit" : "0x1c9c380",
      "gasUsed" : "0xa410",
      "timestamp" : "0x62d92263",
      "extraData" : "0x",
      "baseFeePerGas" : "0x7",
      "blockHash" : "0x13b7dab1660352dad22bcbb7462d03baf3aec68e5cc51bf599daccb21a2b79f7",
      "transactions" : [ "0xf86180820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8026a0b7b0cc34f06e99da2a0eb3f290be06fa5982e5b7883b9d2a46e09ee03861955ba008972a7505395050eb78e332d811049c824534a46d751b8305e1b3f819533017", "0xf86101820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960c8026a096f3751f75a5eeb8f2e27167619ae24efcbb26cf1f5ee6d501ace868398c27dca0740ebd0912eae820d99083c671cf6a483b229a06e28d5e7a215b617cad24f28f" ]
    },
    "unprocessedTransactions" : [ "0xf86301820bb88405f5e10094f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8025a072d6b19aba780fdeb57fab5302bf142c5216f45c845267dca77f9d3e20910d44a05390bc4260c188e55a571f1d6a06ff9168391d4c8a7a498a2db49e41063f4b77" ],
    "invalidTransactions" : [ {
      "transaction" : "0xf8610a820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f960a8025a09f0f2f41a2a7228d342b81f3937441a0767e5d78c25c86a8e5e5bec7e5fd3b33a02775ee8f94d673774f7f6fd090fa4ccd15b797a47236d59c0ad83549191660e4",
      "reason" : "INCORRECT_NONCE",
      "errorMessage" : "transaction nonce 10 does not match sender account nonce 1."
    }, {
      "transaction" : "0xf86a01820bb88259d894f1a98bb35ff74fb6eb07c145c233434aee4f1f96890ad78ebc5ac62000008025a0f6aee06079ff380ec5f0ef90f291b10450636698e9a8bf00484cb06d33713eaba01432b9e6739dcd50d4fbb0555be8a10c7aefb77364816b4493acbc608022deaf",
      "reason" : "UPFRONT_COST_EXCEEDS_BALANCE",
      "errorMessage" : "transaction up-front cost 0x00000000000000000000000000000000000000000000000ad78ebc5aca3cdb40 exceeds transaction sender account balance 0x00000000000000000000000000000000000000000000000ad78ebc5ac25eb236"
    } ]
  }
}
```


## Fixed Issue(s)
- #3760

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 10:09:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4145" class=".btn">#4145</a>
            </td>
            <td>
                <b>
                    logging changes for peering
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Signed-off-by: Stefan <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 07:20:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4142" class=".btn">#4142</a>
            </td>
            <td>
                <b>
                    Peering logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Minor changes to logging. 
* add a separate class to log "Process message" in EthProtocolManager, so logging can be tuned separately by class

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 01:15:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4139" class=".btn">#4139</a>
            </td>
            <td>
                <b>
                    22.7.0 snapshot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prep 22.7.0 release 

Prep snapshot of 22.7.0

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 19:18:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4138" class=".btn">#4138</a>
            </td>
            <td>
                <b>
                    22.7.0 rc2 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                22.7.0-RC2 release

Release 22.7.0-RC2 of Hyperledger Besu

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 19:15:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4137" class=".btn">#4137</a>
            </td>
            <td>
                <b>
                    22.7.0 CHANGELOG.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                update changelog for release

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 19:12:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4136" class=".btn">#4136</a>
            </td>
            <td>
                <b>
                    logging additions for better engine visibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
revamps some of the engine logging for better visibility

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 17:55:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4135" class=".btn">#4135</a>
            </td>
            <td>
                <b>
                    Remove Sonar Integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Sonar has been removed from the build workflow. This PR removes all
configuration and code markings that were used to facilitate it.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 14:28:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4134" class=".btn">#4134</a>
            </td>
            <td>
                <b>
                    Add support for LevelDB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fairly quick and dirty implementation of a LevelDB plugin for Besu. It does pass the `AbstractKeyValueStorageTest` tests but is pretty lacking in unit tests otherwise currently.  LevelDB doesn't support columns by default but this adds support via a key prefix - code for that is taken from Teku (and we could pull over the unit tests for it if this is worth pursuing).

It may be better to not simulate columns since I think besu always uses globally unique keys anyway (pruning needs the ability to iterate a single column but pruning isn't exactly useful anyway). That would likely simplify the implementation and may give different performance/space characteristics as well but I haven't tried it.

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 22:22:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4132" class=".btn">#4132</a>
            </td>
            <td>
                <b>
                    Update RocksDB default block cache size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Update RocksDB default block cache size to mitigate a performance regression from #3985.


Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

We can see in the dashboard below that we have some blocks behind with the RocksDB block cache default value 8 MB, and Besu with block cache size 128 MB is performing better (no blocks behind).

<img width="1672" alt="image" src="https://user-images.githubusercontent.com/5099602/179716882-198371bf-97d5-4ed2-a725-6a802830f4ac.png">


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#4128
## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 09:35:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4131" class=".btn">#4131</a>
            </td>
            <td>
                <b>
                    Fix post merge chain reog with invalid block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description

This PR fixes the failing Hive2 engine test `Invalid Ancestor Chain Re-Org, Invalid ReceiptsRoot, Invalid P8', Reveal using sync`

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 08:53:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4130" class=".btn">#4130</a>
            </td>
            <td>
                <b>
                    Useful response improves reputation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                Currently there is no way for peers improve their reputation. With this PR peers improve their reputation when they send a useful response.

Signed-off-by: Stefan <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 07:18:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4126" class=".btn">#4126</a>
            </td>
            <td>
                <b>
                    alternative malloc implementation - jemalloc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Use jemalloc with linux runtimes to better manage rocksdb memory usage.

* add malloc arena max envar to besu startup
* add jemalloc preload envar to besu startup
* add jemalloc lib download to docker jvm images

smoke tested and verified working on:
 Linux x86_64
 Docker linux aarch64 (on OSX M1)

Native OSX ([El Capitan +](https://developer.apple.com/forums/thread/13161https://developer.apple.com/forums/thread/13161)) is not loading jemalloc currently

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
potentially addresses:
#4057

## Documentation
If we end up going with jemalloc as an alternative malloc implementation for besu, we should document the need to have jemalloc installed in your environment, how to do it for each platform.

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 23:05:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4124" class=".btn">#4124</a>
            </td>
            <td>
                <b>
                    applies merge filtering to peers after 2 finalized
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 19:21:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4122" class=".btn">#4122</a>
            </td>
            <td>
                <b>
                    Check status of block propagation manager before starting or stopping
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description
In `DefaultSynchronizer` check if the `BlockPropagationManager` is running before starting or stopping it. This avoids an exception or warning if it is started or stopped more than once respectively.

## Fixed Issue(s)
fixes #4121

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 12:26:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4120" class=".btn">#4120</a>
            </td>
            <td>
                <b>
                    increase the default max message size for p2p messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                The current limit means that we are disconnecting useful peers during syncing.

Signed-off-by: Stefan <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 06:01:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4118" class=".btn">#4118</a>
            </td>
            <td>
                <b>
                    EIP-1153: Transient storage opcodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

- Implement [EIP-1153: Transient storage opcodes](https://eips.ethereum.org/EIPS/eip-1153)
- Create new Shanghai spec for including this feature post Paris.
- Added a new `ByteCodeBuilder` class to make it easier to construct the E2E test cases.

## Eip1153 Tests 🆕

### TStoreEVMOperationTest.java
- [x]  load arbitrary value is 0 at beginning of transaction: `TLOAD(x)` is `0`
- [x]  loading after storing returns the stored value: `TSTORE(x, y)`, `TLOAD(x)` returns `y`
- [x]  loading any other slot after storing to a slot returns 0: `TSTORE(x, y)`, `TLOAD(x + n)` where `n > 0` returns `0`
- [x]  contracts have separate transient storage—loading a slot in a separate contract after storing returns 0: `TSTORE(x, y)`, `CALL(z, ...)`, `TLOAD(x)` returns `0`
- [x]  reentrant calls access the same transient storage: `TSTORE(x, y)`, `CALL(self, ...)`, `TLOAD(x)` returns `y`
- [x]  reentrant calls can manipulate the same transient storage: `TSTORE(x, y)`, `CALL(self, ...)`, `TSTORE(x, z)`, `TLOAD(x)` returns `z`
- [x]  successfully returned calls do not revert transient storage writes: `TSTORE(x, y)`, `CALL(self, ...)`, `TSTORE(x, z)`, `RETURN`, `TLOAD(x)` returns `z`
- [x]  revert undoes the transient storage write from the failed call: `TSTORE(x, y)`, `CALL(self, ...)`, `TSTORE(x, z)`, `REVERT`, `TLOAD(x)` returns `y`
- [x]  revert undoes all the transient storage writes to the same key from the failed call, i.e. applies the modifications in reverse order: `TSTORE(x, y)`, `CALL(self, ...)`, `TSTORE(x, z)`, `TSTORE(x, z + 1)` `REVERT`, `TLOAD(x)` returns `y`
- [x]  revert undoes transient storage writes from inner calls that successfully returned: `TSTORE(x, y)`, `CALL(self, ...)`, `CALL(self, ...)`, `TSTORE(x, y + 1)`, `RETURN`, `REVERT`, `TLOAD(x)` returns `y`
- [x]  delegatecall manipulates transient storage in the context of the current address: `TSTORE(x, y)`, `DELEGATECALL(a, ...)`, `TSTORE(x, z)`, `RETURN`, `TLOAD(x)` returns `z`
- [x]  delegatecall reads transient storage in the context of the current address: `TSTORE(x, y)`, `DELEGATECALL(a, ...)`, `TLOAD(x)` returns `y`
- [x]  transient storage cannot be manipulated in a static context: `TSTORE(x, y)`, `STATICCALL(a, ...)`, `TSTORE(x, z)` reverts
- [x]  transient storage cannot be manipulated in a static context when calling self: `TSTORE(x, y)`, `STATICCALL(self, ...)`, `TSTORE(x, z)` reverts
- [x]  transient storage cannot be manipulated in a nested static context: `TSTORE(x, y)`, `STATICCALL(self, ...)`, `CALL(self, ...)`, `TSTORE(x, z)` reverts
- [x]  Transient storage can be accessed in a static context when calling self`TSTORE(x, y)`, `STATICCALL(self, ...)`, `CALL(self, ...)`, `TLOAD(x)` returns `y`
- [ ] transient storage does not persist beyond a single transaction: TSTORE(x, y), RETURN, (new transaction to same contract), TLOAD(x, y) returns 0 

### TStoreOperationTest.java

- [x] Insufficient gas
- [x] Simple tstore test
- [x] TLoad uninitialized
- [x] TStore/TLoad 
- [x] TStore->TStore->TLoad
- [x] No gas refund

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

Unclear if I should add a new record to the changelog. Please advise.
- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-16 20:44:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4116" class=".btn">#4116</a>
            </td>
            <td>
                <b>
                    post-merge sync and peering fix 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
addresses two sources of problems when syncing a post-merge network:

*  adds a merge-specific 'best peer' comparator rather than the PoW heaviest chain comparator.  This resolves a bug where besu would order its peers incorrectly and report that it did not have any peers with sufficient chain height: `No sync target with sufficient chain height, waiting for peers: {}`

* ensures 'fast' syncs (snap, checkpoint, fast) set the syncState as having reached TTD to satisfy preconditions for backward sync capability.  This fixes a 'stuck' issue where a fast sync would complete and catch up to a post-merge finalized block, but backward sync was not able to backfill from head back to the finalized block, and besu would just sit at its final fast sync pivot block.
 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#3956
#3329

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-16 08:44:34 +0000 UTC
    </div>
</div>

