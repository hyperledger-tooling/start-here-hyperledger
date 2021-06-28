---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/go-perun/issues/54" class=".btn">54</a>
            </td>
            <td>
                <b>
                    eth/channel/test: Replace custom genesis code in `SimulatedBackend` constructor with `core.DeveloperGenesisBlock`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">good first issue</span><span class="chip">help wanted</span>
            </td>
            <td>
                Our [constructor](https://github.com/hyperledger-labs/go-perun/blob/25e0d303ebf6be4f658f3efa8d596512c0f49cff/backend/ethereum/channel/test/simulated.go#L47) still uses some, now outdated, copied code from [`core.DeveloperGenesisBlock`](https://github.com/ethereum/go-ethereum/blob/d8ff53dfb8a516f47db37dbc7fd7ad18a1e8a125/core/genesis.go#L399). We should use this function instead (passing it as faucet address the key that we generate at the top), avoiding code duplication and being automatically up to date with the latest pre-compiles.

I don't know the meaning of parameter `period`, that's up for research. Looks like it is relevant in our sim backend use case.

Note that the current [gas limit](https://etherscan.io/chart/gaslimit) seems to be 12.5 Mio (with a jump today to 14 Mio?).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 08:43:45 +0000 UTC
    </div>
</div>

