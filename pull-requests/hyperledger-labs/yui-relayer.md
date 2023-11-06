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
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    core: remove `clientID` from CreateMsgCreateClient
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The clientID is determined during Tx execution on chain, so it cannot be specified externally.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 08:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/120" class=".btn">#120</a>
            </td>
            <td>
                <b>
                    fix height flag type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                height flag should be specified as uint64, but int64 is used
- https://github.com/hyperledger-labs/yui-relayer/blob/main/cmd/query.go#L52
- https://github.com/hyperledger-labs/yui-relayer/blob/main/cmd/query.go#L89
- https://github.com/hyperledger-labs/yui-relayer/blob/main/cmd/query.go#L122
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 14:23:09 +0000 UTC
    </div>
</div>

