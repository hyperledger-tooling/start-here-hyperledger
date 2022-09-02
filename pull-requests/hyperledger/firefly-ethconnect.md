---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/229" class=".btn">#229</a>
            </td>
            <td>
                <b>
                    Remove early FFCAPI implementation not it is replaced by EVMConnect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly-evmconnect and https://github.com/hyperledger/firefly-transaction-manager
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 04:34:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/228" class=".btn">#228</a>
            </td>
            <td>
                <b>
                    Two phase init was not passing smartContractGW to receipt store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Which meant no WS receipts were being delivered.

This was caused by new initialization order in #227 

Found through e2e in FireFly under https://github.com/hyperledger/firefly/pull/1033
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 02:25:32 +0000 UTC
    </div>
</div>

