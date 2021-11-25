---
layout: default
title: indy-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk
---

# indy-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2452" class=".btn">#2452</a>
            </td>
            <td>
                <b>
                    Added implementation of MultiWalletMultiTable postgres plugin strategy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We saw that the strategy MultiWalletMultiTable was prepared in the code but not yet implemented.

So decided to do that because we experienced some major peformance issues with the implemented strategies so far.

In addition we added another Strategy: MultiWalletSplitDatabaseMultiTable which cluster the tables in different databases depending on the id of the wallet. That lead to a performance boost.

All unit test ran successfull and we tested the strategy in production aswell but we still consider it as experimentall because further tests are required to ensure that there are no undetected misconceptions.

Signed-off-by: Johannes Henrich <j.henrich@esatus.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 10:00:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2448" class=".btn">#2448</a>
            </td>
            <td>
                <b>
                    iOS wrapper: Fix message is undeliverable issue.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Passing empty `sender` string into `indy_pack_message` can causes failed packing message.

This changes will add string length checking.

https://github.com/hyperledger/aries-framework-javascript/issues/522
https://github.com/hyperledger/aries-mobile-agent-react-native/issues/112
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 10:13:58 +0000 UTC
    </div>
</div>

