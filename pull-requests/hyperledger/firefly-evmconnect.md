---
layout: default
title: firefly-evmconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-evmconnect
---

# firefly-evmconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-evmconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    surface `ErrorNotFound` in get_block_info
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Instead of swallowing `ErrorNotFound` for `blockRPCMethods`, surface it for consumers to decide how to handle the error. Also updated the evmconnect blocklistener implementation to not exit the loop on this error.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 01:36:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Leveraging FFTM's Sprig Support in gasOracle.template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to https://github.com/hyperledger/firefly-transaction-manager/pull/29 and https://github.com/hyperledger/firefly-transaction-manager/pull/30
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 16:52:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    Latest ffsigner and fftm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly-signer/pull/20
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 15:46:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/18" class=".btn">#18</a>
            </td>
            <td>
                <b>
                    fftm version 0.9.8
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
        Created At 2022-08-24 20:17:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Use shared RPC client from firefly-signer library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR depends on https://github.com/hyperledger/firefly-signer/pull/19. It uses the shared RPC client code there instead of duplicating this code in evmconnect as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 15:47:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    update fftm to v0.9.7
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
        Created At 2022-08-23 21:29:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    introduce mapping for block not found errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Encountered this during my testing with avalanche. 

Instead of returning empty block info for an unknown/unvalidated block, some evm blockchains will return an error. Now, the ethereum connector can keep track of these different errors and treat them as if `blockInfo` is `nil`

 in a chain with #11 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 14:08:40 +0000 UTC
    </div>
</div>

