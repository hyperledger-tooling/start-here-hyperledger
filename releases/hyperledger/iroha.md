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
                    Hyperledger Iroha v1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    1.4.0
                </span>
            </td>
            <td>
                Since 1.3 the team implemented the following features and fixes:

## Features

### Syncing Node #1648
Adds syncing node state for Iroha.
<details>
	<summary>What is a syncing node?</summary>

Node in the state can:
- send transactions
- execute queries
- synchronize with remote nodes
- apply and validate blocks
- construct WSV

It can not:
- request proposals
- send votes(votes from such a node will be skipped)
- generate events of building block
</details>

### RocksDB Metrics #1692

### Healthcheck #1735
Added healthcheck interfaces via:
- http
- grpc
- metrics

## General Fixes
Iroha v1.4-rc.1 fixes #1785 :
- Drop wsv flag behavior
- Signatory case insensetive checks
- Transaction status description from 5 byte to 1 byte if true or 0 byte if false
- Bloom filter in RDB
- RadixTrie enumerates nodes by prefix filter
- RDB 2-layer cache for WSV

Iroha v1.4-rc.2 fixes #1824 :
- Switched from optimistic to transactions database in RocksDB
- WSV and block store are now in different column families
- WSV schema version increased to 1.4.0

GitHub Action Docker tag #1609

Fixed sample config files (from max_rounds_delay to proposal_creation_timeout and deprecated DB connection string) #1662

## Docs Fixes
Fixed broken links: build status, build guide, etc.  #1318 
Small Fixes on Configuration and Docker Metrics #1654
Added missing dependencies: #1393


            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/iroha/releases/tag/1.4.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-01-31 06:28:46 +0000 UTC
    </span>
</div>

