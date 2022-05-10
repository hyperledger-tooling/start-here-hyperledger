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
                    Hyperledger Iroha v1.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    1.5.0
                </span>
            </td>
            <td>
                Here are the changes compared to HL Iroha 1.4:

## Features

RocksDB Storage Implementation for Burrow #2065

Removed proposal_delay timeout (now is set automatically as `2 * proposal_creation_timeout` based on the calculations of the optimal value of the proposal delay) #1847

## Performance Improvement

Removed separate MST endpoint: MST module is now located in the Ordering Service module to improve the performance #1927

Proposal request optimization #1869 #1971

## Documentation

Documentation on Healthcheck Endpoint, Iroha Swarm, RocksDB and Postgres comparison and an example of good migration practice #1935
Documentation build fix #2069

## Infrastructure

Removed Jenkins-related files as a part of moving CI to GitHub Actions #1921 
More changes in CI can be seen [here](https://github.com/hyperledger/iroha/compare/1.4.0...1.5.0)

Docker image existence flag fix #1901

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/iroha/releases/tag/1.5.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-04-08 12:46:44 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Iroha v2.0.0-pre-rc.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.0.0-pre-rc.3
                </span>
            </td>
            <td>
                - Schema changes that fix https://github.com/hyperledger/iroha/issues/1969
- Schema endpoint (use curl -X GET http://127.0.0.1:8080/schema)
- WASM decode optimisations
- timed triggers
- Improved API for generating ISI (documentation pending)
- By-call triggers
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/iroha/releases/tag/v2.0.0-pre-rc.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-03-31 11:17:36 +0000 UTC
    </span>
</div>

