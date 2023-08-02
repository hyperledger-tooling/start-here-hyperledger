---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/99" class=".btn">#99</a>
            </td>
            <td>
                <b>
                    Fixing a nonce conflict issue when the cached nonce expired.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is a problem when two different batches of transaction inserts happen in parallel, one of them will read the incorrect nonce back from the DB + the nonce callback when the cached nonce expires. 

The fix in the PR is to check the expired cached nonce first to avoid pending transactions that have clashing nonces between them.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 07:46:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/98" class=".btn">#98</a>
            </td>
            <td>
                <b>
                    avoid using internal interface in public pkg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In order to using mockery in another golang module, we need to make sure the interfaces are defined in the external packages and consumed by the internal interface, not the other way around. 

Otherwise the consumer will hit problem like the following:
<img width="1523" alt="image" src="https://github.com/hyperledger/firefly-transaction-manager/assets/5425125/48ba106e-fd11-4661-af68-bf44241f5f63">

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 15:32:49 +0000 UTC
    </div>
</div>

