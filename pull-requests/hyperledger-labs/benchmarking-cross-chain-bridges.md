---
layout: default
title: benchmarking-cross-chain-bridges
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/benchmarking-cross-chain-bridges
---

# benchmarking-cross-chain-bridges <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    feat: socket benchmarking
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Done:
1. Socket benchmarking  - cross-chain trades
2. Socket routing generates same and cross-chain routes 

Fix:
1.  foundry.toml to match forge 

Todo:
1. Socket same chain trade parser
2. Add parser for message-aggregators
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 16:17:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    feat: xy and uniswap benchmarkers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Done:
1. Benchmarking XY 
2. Added Uniswap Universal Router to uniswap route_builder
3. Benchmarking Uniswap Swap Router V2 and Universal Router

Refactor: 
1. Move benchmarks from src/benchmark/protocol to src/benchmark/-aggregator/protocol

Remove: 
1. Sushiswap from token-aggregators

Packages removed:
1. @sushiswap/sdk 
2. @uniswap/universal-router-sdk

Todo:
1. Get socket to work (contact team)
2. Setup XY for same chain swaps
3. Add message-aggregators
4. Perform live network benchmarks
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-26 16:37:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges/pull/14" class=".btn">#14</a>
            </td>
            <td>
                <b>
                    feat: benchmarking cowswap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Done:
1. Benchmarking cowswap
2. Additional benchmarks for lifi
3. Using coingecko api to fetch token price in usd
4. Created custom datatype Token that stores token type (native, stable, wrapped) and decimals

Fix:
1. Lifi mainnet url changed from li.quest to staging.li.quest
2. Bug where cowswap wouldn't use the right url for non goerli trades

Refactor:
1. Reports generated into benchmark-data/protocol/source_chain_name/dest_chain_name


Package Install:
"@cowprotocol/cow-sdk": "4.0.3"
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 16:18:14 +0000 UTC
    </div>
</div>

