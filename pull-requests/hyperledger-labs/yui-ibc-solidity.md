---
layout: default
title: yui-ibc-solidity
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-ibc-solidity
---

# yui-ibc-solidity <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-ibc-solidity){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/76" class=".btn">#76</a>
            </td>
            <td>
                <b>
                    Fix IBCHeight.toUint128
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix a bug related to operator precedence.
https://docs.soliditylang.org/en/v0.8.9/cheatsheet.html

`x << 64 + y` means `x << (64 + y)`, not `(x << 64) + y`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-14 07:17:47 +0000 UTC
    </div>
</div>

