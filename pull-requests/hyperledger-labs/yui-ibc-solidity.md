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
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/150" class=".btn">#150</a>
            </td>
            <td>
                <b>
                    Separate the packet functions from IBCChannel.sol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The contract size of the IBCChannel reaches near size limit of ethereum, so it is difficult to implement additional new features(e.g. #12). Therefore, we try to work around the limit by separating the contract into two components, one for the handshake functions and the other for the packet functions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-18 10:43:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/148" class=".btn">#148</a>
            </td>
            <td>
                <b>
                    ics-02: Add verifyNonMembership support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                related to #12
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-18 05:17:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/147" class=".btn">#147</a>
            </td>
            <td>
                <b>
                    Use openzeppelin's Strings.sol
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
        Created At 2022-12-15 14:51:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/146" class=".btn">#146</a>
            </td>
            <td>
                <b>
                    Use solidity-rlp with npm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix https://github.com/hyperledger-labs/yui-ibc-solidity/issues/144

Signed-off-by: Jun Kimura <jun.kimura@datachain.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-15 00:57:47 +0000 UTC
    </div>
</div>

