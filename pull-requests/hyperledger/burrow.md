---
layout: default
title: burrow
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/burrow
---

# burrow <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/burrow){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/burrow/pull/1488" class=".btn">#1488</a>
            </td>
            <td>
                <b>
                    Fixed RLP encoding extra leading zeros on uint64
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When a uint64 fits perfectly in a multiple 8 bits, a leading zero was being added to the encoded value, for example 233 was encoded (prefix elided) as `00 e9` while it should have been `e9`

Simply changed the way the amount of byte required is computed so the right amount of leading zeros is correctly removed after encoding.

For uint64 value <= 255, this will even save an allocation since we will more often enter the `encodeUint8` case which is faster (theorically).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 03:27:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/burrow/pull/1487" class=".btn">#1487</a>
            </td>
            <td>
                <b>
                    Pull solts into Burrow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In preparation for built-in Solidity codegen

Signed-off-by: Silas Davis <silas@monax.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-16 11:55:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/burrow/pull/1486" class=".btn">#1486</a>
            </td>
            <td>
                <b>
                    Get rid of excessively long and generally useless EVM trace from call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                errors

Signed-off-by: Silas Davis <silas@monax.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-15 21:16:05 +0000 UTC
    </div>
</div>

