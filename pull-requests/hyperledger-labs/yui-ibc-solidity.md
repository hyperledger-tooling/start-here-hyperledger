---
layout: default
title: yui-ibc-solidity
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-ibc-solidity
---

# yui-ibc-solidity <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-ibc-solidity){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/41" class=".btn">#41</a>
            </td>
            <td>
                <b>
                    Emit the event `WriteAcknowledgement` in RecvPacket
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 05:51:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/39" class=".btn">#39</a>
            </td>
            <td>
                <b>
                    Use protobuf-any type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 04:35:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/37" class=".btn">#37</a>
            </td>
            <td>
                <b>
                    Fix to use a valid client identifier for IBC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>

In ics-024, the length of Client identifier must be greater than or equal to 9.

ref. 
https://github.com/cosmos/ibc/tree/master/spec/core/ics-024-host-requirements#paths-identifiers-separators
https://github.com/cosmos/ibc-go/blob/fa091bcda3b1dbbf687ff4465f9fd309a4206e67/modules/core/24-host/validate.go#L61
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 02:44:05 +0000 UTC
    </div>
</div>

