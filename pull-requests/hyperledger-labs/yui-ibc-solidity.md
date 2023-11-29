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
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/236" class=".btn">#236</a>
            </td>
            <td>
                <b>
                    Bump up minimal solidity version to v0.8.12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Before v0.8.12, there is an internal compiler error of casting `string(b[from:to])` where type of b is `bytes calldata`. Therefore, ICS-20 that uses this cast cannot be compiled with <v0.8.12 at least.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 09:10:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/235" class=".btn">#235</a>
            </td>
            <td>
                <b>
                    Improve linter settings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - bump up solhint to v4
- enable two further lint rules: `no-unused-import`, `no-global-import`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 00:56:32 +0000 UTC
    </div>
</div>

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

