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
                    23.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    23.4.1
                </span>
            </td>
            <td>
                Besu 23.4.1 is an optional update for proof of stake and has a variety of enhancements.
* A new (optional/experimental) tx pool format that builds great, more profitable local blocks if you are not using MEV-boost. 
* Networking / peering updates
* Database storage reductions
* Fixes for dockers and RPC
* Mainnet Cancun fork development

### Breaking Changes
- Add request content length limit for the JSON-RPC API (5MB) [#5467](https://github.com/hyperledger/besu/pull/5467)
- `min-block-occupancy-ratio` options is now ignored on PoS networks [#5491](https://github.com/hyperledger/besu/pull/5491)

### Additions and Improvements
- Set the retention policy for RocksDB log files to maintain only the logs from the last week [#5428](https://github.com/hyperledger/besu/pull/5428)
- "Big-EOF" (the EOF version initially slotted for Shanghai) has been moved from Cancun to FutureEIPs [#5429](https://github.com/hyperledger/besu/pull/5429)
- EIP-4844: Zero blob transactions are invalid [#5425](https://github.com/hyperledger/besu/pull/5425)
- Transaction pool flag to disable specific behaviors for locally submitted transactions [#5418](https://github.com/hyperledger/besu/pull/5418)
- New optional feature to save the txpool content to file on shutdown and reloading it on startup [#5434](https://github.com/hyperledger/besu/pull/5434)
- New option to send SNI header in TLS ClientHello message [#5439](https://github.com/hyperledger/besu/pull/5439)
- Early access - layered transaction pool implementation [#5290](https://github.com/hyperledger/besu/pull/5290)
- New RPC method `debug_getRawReceipts` [#5476](https://github.com/hyperledger/besu/pull/5476)
- Add TrieLogFactory plugin support [#5440](https://github.com/hyperledger/besu/pull/5440)
- Ignore `min-block-occupancy-ratio` option when on PoS networks, since in some cases, it prevents to have full blocks even if enough transactions are present [#5491](https://github.com/hyperledger/besu/pull/5491) 

### Bug Fixes
- Fix eth_feeHistory response for the case in which blockCount is higher than highestBlock requested. [#5397](https://github.com/hyperledger/besu/pull/5397)
- Fix Besu Docker image failing to start due to NoClassDefFoundError with org.xerial.snappy.Snappy library. [#5462](https://github.com/hyperledger/besu/pull/5462)

### Download Links

- https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.4.1/besu-23.4.1.tar.gz / sha256: 49d3a7a069cae307497093d834f873ce7804a46dd59207d5e8321459532d318e
- https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/23.4.1/besu-23.4.1.zip / sha256: 1d82ed83a816968aa9366d9310b275ca6438100f5d3eb1ec03d3474b2a5f5e76

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/23.4.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-05-26 04:07:37 +0000 UTC
    </span>
</div>

