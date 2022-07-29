---
layout: default
title: fabric-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-go
---

# fabric-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/244" class=".btn">#244</a>
            </td>
            <td>
                <b>
                    feat: expose ChannelProvider from the gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We have a use case where given a Getway we need to query the ledger for some information (retrieving block from txID).

Being able to obtain the ChannelProvider is convenient since we can then create ledger.Client as needed.
I wonder however if it is desirable to expose such a low level component. Maybe something like `gateway.GetLedger(...)` would be more appropriate? Let me know what you think.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-29 08:59:14 +0000 UTC
    </div>
</div>

