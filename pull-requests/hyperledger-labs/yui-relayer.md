---
layout: default
title: yui-relayer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-relayer
---

# yui-relayer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-relayer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    Update path config IDs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Add SendMsgs
* Removed required checks for ClientID and ConnectionID
* Remove overWriteConfig
* Add configI to core package

This allows the client-id, connection-id, and channel-id in path.json to be set to empty by default.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-24 09:12:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    change interfaces related to MsgCreateClient
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - replace `LightClient::CreateMsgCreateClient` with `CreateInitialLightClientState`
- remove `FinalityAware::GetFinalizedHeader`
- restore `FinalityAware::GetLatestFinalizedHeader`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 07:43:34 +0000 UTC
    </div>
</div>

