---
layout: default
title: caliper-benchmarks
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper-benchmarks
---

# caliper-benchmarks <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper-benchmarks){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/223" class=".btn">#223</a>
            </td>
            <td>
                <b>
                    Fix Besu docker compose network bug (#222)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #222 
Fixes #172

* Remove custom Dockerfile for building the Besu node
* Use the official image directly, and anchored to a specific version
* Update CLI options (fixing rpc-ws-apis bug and adhering to inclusive language statement), essentially syncing it with the Caliper CI test

Signed-off-by: Attila Klenik <a.klenik@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 14:46:04 +0000 UTC
    </div>
</div>

