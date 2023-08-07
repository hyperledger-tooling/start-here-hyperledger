---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1476" class=".btn">#1476</a>
            </td>
            <td>
                <b>
                    Link to the Solana getting started guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/solang/issues/1475.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-07 08:02:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1474" class=".btn">#1474</a>
            </td>
            <td>
                <b>
                    Represent contracts by their program id
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
        Created At 2023-08-04 20:24:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1473" class=".btn">#1473</a>
            </td>
            <td>
                <b>
                    Updates for Solidity 0.8.21
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solidity introduces an experimental feature:

	pragma experimental solidity;

	import std.stub;

Note it is not supported yet, but we've added it to the Solidity parser and formatter, and Solang now gives nice error messages when it encounters these.

Note that the evm test failures have gone up, but this is not a regression. There are simply more tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-01 13:11:16 +0000 UTC
    </div>
</div>

