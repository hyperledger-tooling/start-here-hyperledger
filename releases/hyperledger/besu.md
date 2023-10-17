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
                    23.10.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.10.0
                </span>
            </td>
            <td>
                ## 23.10.0
### Layered Transaction Pool: the new default transaction pool implementation
With this release the previously experimental Layered txpool is marked stable and enabled by default, so please read the following instructions if you used to tune txpool behavior, otherwise you can simply go with the default and enjoy the improved performance of the new txpool. More detailed information about the implementation of the [Layered TxPool can be found here](https://github.com/hyperledger/besu/pull/5290).

#### Upgrading to Layered Transaction Pool
If you do not specify any txpool option, then you can skip this section.
If you have tuned the txpool using one of these options: `tx-pool-retention-hours`, `tx-pool-limit-by-account-percentage` or `tx-pool-max-size`,
then you need to update your configuration as described below:
- `tx-pool-retention-hours`: simply remove it, since it is not applicable in the Layered txpool, old transactions will eventually expire when the memory cache is full.
- `tx-pool-limit-by-account-percentage`: replace it with `tx-pool-max-future-by-sender`, which specify the max number of sequential transactions of single sender are kept in the txpool, by default it is 200.
- `tx-pool-max-size`: the Layered txpool is not limited by a max number of transactions, but by the estimated memory size the transactions occupy, so you need to remove this option, and to tune the max amount of memory<sup>*</sup> use the new option `tx-pool-layer-max-capacity` as described below.

You can still opt-out of the Layered txpool, setting `tx-pool=legacy` in config file or via cli argument, but be warned that the Legacy implementation will be deprecated for removal soon, so start testing the new implementation.

#### Configuring the Layered Transaction Pool
By default, the txpool is tuned for mainnet usage, but if you are using private networks or want to otherwise tune it, these are the new options:
- `tx-pool-max-future-by-sender`: specify the max number of sequential transactions of a single sender are kept in the txpool, by default it is 200, increase it to allow a single sender to fit more transactions in a single block. For private networks, this can safely be set in the hundreds or thousands if you want to ensure future transactions (with large nonce gaps) remain in the pool.
- `tx-pool-layer-max-capacity`: set the max amount of memory<sup>*</sup> in bytes, a single memory limited layer can occupy, by default is 12.5MB, keep in mind that there are 2 memory limited layers, so the expected memory consumption is twice the value specified by this option, so 25MB by default. Increase this value if you have spare RAM and the eviction rate is high for your network.
- `tx-pool-max-prioritized`: set the max number of transactions allowed in the first layer, that only contains transactions that are candidate for inclusion in the next block creation task. It makes sense to limit the value to the max number of transactions that fit in a block in your network, by default is 2000.

<sup>*</sup>: the memory used by the txpool is an estimation, we are working to make it always more accurate.

### Breaking Changes
- Removed support for Kotti network (ETC) [#5816](https://github.com/hyperledger/besu/pull/5816)
- Layered transaction pool implementation is now stable and enabled by default, so the following changes to experimental options have been done #5772:
    - `--Xlayered-tx-pool` is gone, to select the implementation use the new `--tx-pool` option with values `layered` (default) or `legacy`
    - `--Xlayered-tx-pool-layer-max-capacity`, `--Xlayered-tx-pool-max-prioritized` and `--Xlayered-tx-pool-max-future-by-sender` just drop the `X` and keep the same behavior

### Additions and Improvements
- Add access to an immutable world view to start/end transaction hooks in the tracing API[#5836](https://github.com/hyperledger/besu/pull/5836)
- Layered transaction pool implementation is now stable and enabled by default. If you want still to use the legacy implementation, use `--tx-pool=legacy`. 
  By default, the new transaction pool is capped at using 25MB of memory, this limit can be raised using `--layered-tx-pool-layer-max-capacity` options #5772
- Tune G1GC to reduce Besu memory footprint, and new `besu-untuned` start scripts to run without any specific G1GC flags [#5879](https://github.com/hyperledger/besu/pull/5879)
- Reduce `engine_forkchoiceUpdatedV?` response time by asynchronously process block added events in the transaction pool [#5909](https://github.com/hyperledger/besu/pull/5909) 

### Bug Fixes
- do not create ignorable storage on revert storage-variables subcommand [#5830](https://github.com/hyperledger/besu/pull/5830) 
- fix duplicate key errors in EthScheduler-Transactions [#5857](https://github.com/hyperledger/besu/pull/5857)
- Don't put control characters, escaped or otherwise, in t8n stacktraces [#5910](https://github.com/hyperledger/besu/pull/5910)

### Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.10.0/besu-23.10.0.tar.gz / sha256: 3c75f3792bfdb0892705b378f0b8bfc14ef6cecf1d8afe711d8d8687ed6687cf

https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/23.10.0/besu-23.10.0.zip / sha256: d5dafff4c3cbf104bf75b34a9f108dcdd7b08d2759de75ec65cd997f38f52866
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.10.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-10-10 17:16:38 +0000 UTC
    </span>
</div>

