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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Misc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add:
1. yarn clear { :benchmarks, :run-data, :all }
2. Skip XY test that executes route

Fix:
1. XY:execute_route error handling
2.  console.log() -> console.error() wherever applicable
3. Lifi uses ETH and not WETH for testnet swaps

Upgrade:
"@lifi/sdk": "2.4.3" -> "2.5.0"
"@types/node": "20.8.8" -> "20.9.4"
"@uniswap/smart-order-router": "3.17.2" -> "3.19.0"
"typescript": "5.2.2" -> "5.3.2"
"@types/chai": "4.3.9" -> "4.3.11"
"@types/mocha": "10.0.3" -> "10.0.6"

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 22:37:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/benchmarking-cross-chain-bridges/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Benchmark init + Benchmark LiFi
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Done:
1. Created benchmark framework (alpha)
2. Benchmarking lifi on mainnet and testnet based off api results 
3. Lifi transaction typings 
4. Provider functions to get latest block and gas price
5. Support for Polygon mainnet

Fix:
1. Lifi dropped support for WETH trades on testnet (no longer fails test)
2. Socket testing skips when user address has low funds 

Misc:
1. Rename @benchmarking-cross-chain-bridges/helper/token-misc to @benchmarking-cross-chain-bridges/helper/token_misc 

Todo: 
1. Live transaction benchmark with latencies
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 21:47:15 +0000 UTC
    </div>
</div>

