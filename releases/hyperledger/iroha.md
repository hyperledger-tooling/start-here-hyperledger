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
                    Hyperledger Iroha v1.4-rc.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    1.4.0-rc.1
                </span>
            </td>
            <td>
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

## Docs Fixes
Fixed broken links: build status, build guide, etc.  #1318 
Small Fixes on Configuration and Docker Metrics #1654
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/iroha/releases/tag/1.4.0-rc.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-12-29 11:08:04 +0000 UTC
    </span>
</div>

