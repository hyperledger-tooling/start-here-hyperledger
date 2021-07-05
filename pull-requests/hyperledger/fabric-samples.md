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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/455" class=".btn">#455</a>
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
                Add a new sample in typescript to show how to use an HSM within a client node application

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-30 09:56:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/454" class=".btn">#454</a>
            </td>
            <td>
                <b>
                    expose operations endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 17:59:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/453" class=".btn">#453</a>
            </td>
            <td>
                <b>
                    expose operations endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 17:50:37 +0000 UTC
    </div>
</div>

