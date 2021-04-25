---
layout: default
title: iroha-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-python
---

# iroha-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/69" class=".btn">#69</a>
            </td>
            <td>
                <b>
                    Add possibility of checking transaction status by hash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I noticed that sometimes statuses are not receiving in timeout, if it happen it is really hard to find out what was reason of the transaction if it is not committed - is it still pending, or it was rejected.
So I've decided that it would be really useful if iroha-python has functionality as `iroha-cli` to check status of transaction.
The functionality is really important for me, because I'm integrating external payment system to transfer tokens to iroha from online-bank-transfer, so I must know if transaction in iroha was COMMITTED, REJECTED, or PENDING to provide proper reaction.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 16:08:16 +0000 UTC
    </div>
</div>

