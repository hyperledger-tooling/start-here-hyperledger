---
layout: default
title: perun-eth-backend
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-eth-backend
---

# perun-eth-backend <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-eth-backend){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-eth-backend/pull/52" class=".btn">#52</a>
            </td>
            <td>
                <b>
                    Egoistic Funding Test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes a test case that:
- tests correctness of SetEgoisticPart
- tests correctness of SetEgoisticChains
- tests funding when one participant is set to be egoistic (funds last)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-26 13:10:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-eth-backend/pull/51" class=".btn">#51</a>
            </td>
            <td>
                <b>
                    feat(wire): add ecdsa authentication to wire
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Wire Identity Authentication

## Description
This PR aims to add the ECDSA cryptographic authentication feature to the `wire`'s implementation of perun-eth-backend. The cryptographic key pair is ECDSA, with a signature length of 65, taking inspiration from the wallet implementation of perun-eth-backend. This implementation must be in sync with the wire interface of go-perun 1.11.

### Location: `wire` package

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-25 09:07:04 +0000 UTC
    </div>
</div>

