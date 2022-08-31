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
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/27" class=".btn">#27</a>
            </td>
            <td>
                <b>
                    Update to firefly-signer v0.9.19
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 14:41:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    Do not uninstall empty filters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Noticed cruft like this in the logs, due to an unnecessary call:

```
[2022-08-30T15:42:10.936Z] ERROR evmconnect: RPC[000001286] <-- ERROR: FF22012: Backend RPC request failed eventstream=0182ef67-007c-7d84-206d-eb3364392daf
[2022-08-30T15:42:10.936Z]  WARN evmconnect: Error uninstalling filter '': FF22012: Backend RPC request failed eventstream=0182ef67-007c-7d84-206d-eb3364392daf
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 21:12:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Allow requesting of looking up the signer, separate from an array of methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on https://github.com/hyperledger/firefly-transaction-manager/pull/32 for EthConnect compatibility, where these options were combined.

> Currently this PR pulls in a commit from FFTM until there's a release with PR 32 in it
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 21:13:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Update firefly-signer to v0.9.18
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 19:28:32 +0000 UTC
    </div>
</div>

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

