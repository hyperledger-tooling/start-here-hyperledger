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

