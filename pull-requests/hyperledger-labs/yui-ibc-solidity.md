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
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/258" class=".btn">#258</a>
            </td>
            <td>
                <b>
                    Fix `timeoutPacket` to refer correct timestamp corresponding to `proofHeight`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-26 15:10:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/257" class=".btn">#257</a>
            </td>
            <td>
                <b>
                    Add `getLatestInfo` function to `ILightClient`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Call `getLatestInfo` function instead of calling multiple LightClient contract in `sendPacket` function.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-26 14:26:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    Improve gas cost efficiency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes the following minor improvements
- fix calcBlockDelay to early return if timeDelay is zero
- fix some commitment path generator to accept calldata argument
- split capabilities into portCapabilities and channelCapabilities 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-26 07:51:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    Remove tests using ganache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These test cases are now covered by e2e with HB and solidity test code with forge.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-25 04:34:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-ibc-solidity/pull/254" class=".btn">#254</a>
            </td>
            <td>
                <b>
                    Add `Packet` struct instead of proto generated code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes
- add `Packet` struct
- remove unused proto definitions and generated code
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-25 02:53:35 +0000 UTC
    </div>
</div>

