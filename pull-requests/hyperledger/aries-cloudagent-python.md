---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1453" class=".btn">#1453</a>
            </td>
            <td>
                <b>
                    Update base record time-stamp to standard ISO format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR solves issue #1449 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 08:32:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1450" class=".btn">#1450</a>
            </td>
            <td>
                <b>
                    Endorser protocol askar fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add askar support to integration test script (`BDD_EXTRA_AGENT_ARGS="{\"wallet-type\":\"askar\"}" ./demo/run_bdd`)

Fix database locking errors (similar issues as were fixed in PR https://github.com/hyperledger/aries-cloudagent-python/pull/1439)

Fix/cleanup unit tests

- unit tests are all passing
- `./run_bdd` all tests pass (indy-sdk, default wallet)
- `ACAPY_ARG_FILE=postgres-indy-args.yml ./run_bdd` all tests pass (indy-sdk, postgres wallet)
- `BDD_EXTRA_AGENT_ARGS="{\"wallet-type\":\"askar\"}" ./run_bdd` all tests pass (askar/credx, default wallet)
- `BDD_EXTRA_AGENT_ARGS="{\"wallet-type\":\"askar\"}" ACAPY_ARG_FILE=postgres-indy-args.yml ./run_bdd` all tests pass (askar/credx, postgres wallet)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 13:48:57 +0000 UTC
    </div>
</div>

