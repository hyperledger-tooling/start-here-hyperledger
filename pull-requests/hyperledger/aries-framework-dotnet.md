---
layout: default
title: aries-framework-dotnet
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-dotnet
---

# aries-framework-dotnet <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-dotnet){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-dotnet/pull/243" class=".btn">#243</a>
            </td>
            <td>
                <b>
                    adjust HttpMessageDispatcher to support content type "application/didcomm-envelope-enc"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Short description of what this resolves:
Adds support for content type "application/didcomm-envelope-enc" and supports fallback values as described here: https://github.com/hyperledger/aries-rfcs/blob/main/features/0025-didcomm-transports/README.md

#### Changes proposed in this pull request:
- Adds support for content type "application/didcomm-envelope-enc"
- supports fallback to "application/ssi-agent-wire" and "application/json"
- uses the same content type as the request for the response 

**Fixes**: #

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 21:10:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-dotnet/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    add UpsertDeviceInfoMessage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Short description of what this resolves:
Adds support to update existing DeviceInfoRecords with an UpsertDeviceMessage.

#### Changes proposed in this pull request:
- Adds support to update existing DeviceInfoRecords with an UpsertDeviceMessage.

**Fixes**: #

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 21:04:51 +0000 UTC
    </div>
</div>

