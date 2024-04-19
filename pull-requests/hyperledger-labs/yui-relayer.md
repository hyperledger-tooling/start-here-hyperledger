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
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/139" class=".btn">#139</a>
            </td>
            <td>
                <b>
                    [bugfix] Fix handling error returned from `QueryClientStatePair`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR also does:
- Fix some other error handling
- Delete some unused code
- Update buf (protobuf) stuffs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-18 22:26:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/138" class=".btn">#138</a>
            </td>
            <td>
                <b>
                    Change behaviors of create client, connection, and channel commands.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - just exit with status 1 if config.json has id but that client/connection/channel is not exists.
 - just exit with status 0 if config.json has id and that client/connection/channel is already opened.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-13 18:44:25 +0000 UTC
    </div>
</div>

