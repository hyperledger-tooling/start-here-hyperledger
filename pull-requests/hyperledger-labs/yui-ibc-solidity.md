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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    Fix the module path
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>

fixed #35 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-18 03:31:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    Fix to verify a clientstate in connection handshake
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>

related to #33 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-18 00:21:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    Fix to verifyPacketAcknowledgement receive the original data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>

fixed #30 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-17 11:41:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    Improve the portability of Mock client spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change is also intended to be used for the purpose of checking the compatibility of two different IBC implementations. (e.g. between ibc-solidity and ibc-go)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 22:44:21 +0000 UTC
    </div>
</div>

