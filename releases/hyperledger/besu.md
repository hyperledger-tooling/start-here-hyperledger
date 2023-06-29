---
layout: default
title: besu
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    23.4.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.4.4
                </span>
            </td>
            <td>
                Besu 23.4.4 is an optional update for proof of stake and has a variety of enhancements
- ***NOTE*** A DB migration is performed at startup. To prepare your node for a rollback you need to run Besu with the subcommand `storage revert-variables` with the same configuration used to run Besu. 
- The new experimental healing mechanism for the flat db aims to improve the performance of your node by enabling faster block processing time. Since the processing time will be faster, you should further reduce the chances of missing attestations, making your validator even better. The cost of this feature is a slightly larger database size and a slightly longer sync time. For more detail see https://github.com/hyperledger/besu/pull/5319

### Breaking Changes
- Move blockchain related variables in a dedicated storage, to pave the way to future optimizations [#5471](https://github.com/hyperledger/besu/pull/5471). The migration is performed automatically at startup,
and in case a rollback is needed, before installing a previous version, the migration can be reverted, using the subcommand `storage revert-variables` with the same configuration used to run Besu.
- Remove deprecated Rinkeby named network. [#5540](https://github.com/hyperledger/besu/pull/5540)

### Additions and Improvements
- Allow Ethstats connection url to specify ws:// or wss:// scheme. [#5494](https://github.com/hyperledger/besu/issues/5494)
- Add support for Shanghai changes to the GraphQL service [#5496](https://github.com/hyperledger/besu/pull/5496)
- Unite the tx-pool CLI options under the same Tx Pool Options group in UX. [#5466](https://github.com/hyperledger/besu/issues/5466)
- Tidy DEBUG logs by moving engine API full logging to TRACE [#5529](https://github.com/hyperledger/besu/pull/5529)
- Remove PoW validation if merge is enabled as it is not needed anymore [#5538](https://github.com/hyperledger/besu/pull/5538)
- Use BlobDB for blockchain storage to reduce initial sync time and write amplification [#5475](https://github.com/hyperledger/besu/pull/5475)
- Update to Tuweni 2.4.1. [#5513](https://github.com/hyperledger/besu/pull/5513)
- Add healing flat db mechanism with experimental CLI options `--Xsnapsync-synchronizer-flat-db-healing-enabled=true` [#5319](https://github.com/hyperledger/besu/pull/5319)

### Bug Fixes
- Fix backwards sync bug where chain is rolled back too far, especially when restarting Nimbus [#5497](https://github.com/hyperledger/besu/pull/5497)
- Check to ensure storage and transactions are not closed prior to reading/writing [#5527](https://github.com/hyperledger/besu/pull/5527) 
- Fix the unavailability of account code and storage on GraphQl/Bonsai [#5548](https://github.com/hyperledger/besu/pull/5548)

### Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.4.4/besu-23.4.4.tar.gz / sha256: bd476d235b6fe1f236a62bc709f41c87deb68b72c47bb5b58e56b9d9283af2c4
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.4.4/besu-23.4.4.zip / sha256: 4575000f4fd21d318e7b77340c9281d496bc800bee5b45a13684319e6f28bf27
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.4.4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-28 02:19:07 +0000 UTC
    </span>
</div>

