---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/381" class=".btn">#381</a>
            </td>
            <td>
                <b>
                    update open offsets directory to version 3 from Berkeley carbon trading project
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 00:13:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/380" class=".btn">#380</a>
            </td>
            <td>
                <b>
                    Bump openzeppelin/contracts to 4.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    This commit address a low severity vulnerability in openzeppelin contracts 3.3.0/3.4.1. Should respond to [PR 374](https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/374) and [PR 375](https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/375) 
    Requires upgrading to solidity ^0.8.0 - now using compiler version 0.8.3:
        - Derived contract must override function "supportsInterface" (see new overrides in derived contracts)
        - Require changing getChainId() (DAOToken/Governor contracts) from pure to view
        - uint(-1) changec to type(uint).max
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-03 12:23:52 +0000 UTC
    </div>
</div>

