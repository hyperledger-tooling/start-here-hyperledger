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
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/234" class=".btn">#234</a>
            </td>
            <td>
                <b>
                    Refactoring to merge handler into each feature implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Changes

- merge handler into each feature implementation
- add `IIBCHandler` interface
- remove `IBCMsgs` and move the msg definitions into each feature impl
- add `IBCSelfStateValidator` contract that validates self client/consensus states in the connection handshake
  - developers override this to be able to validate state corresponding to their light client 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 00:44:24 +0000 UTC
    </div>
</div>

