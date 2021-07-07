---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/459" class=".btn">#459</a>
            </td>
            <td>
                <b>
                    chore: minor simplification of configtx yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We dont need << as we are not adding or overwriting any values.

Signed-off-by: ankitm123 <ankitmohapatra123@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 11:22:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/458" class=".btn">#458</a>
            </td>
            <td>
                <b>
                    New HSM Typescript Sample
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a new sample in typescript to show how to use an HSM within a client
node application

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 10:59:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/457" class=".btn">#457</a>
            </td>
            <td>
                <b>
                    Fix off_chain_data to put data to off-chain database
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The off_chain_data sample fails to put data to the off-chain
database. The application does not read fetched blocks because
it uses the old interface of `addBlockListener()` to handle
block events.

This PR fixes the application to use the latest block listener
and build the off-chain database.

Signed-off-by: Yuki Kondo <yuki.kondo.ob@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 05:55:27 +0000 UTC
    </div>
</div>

