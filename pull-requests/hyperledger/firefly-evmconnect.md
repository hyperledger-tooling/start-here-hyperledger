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
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    GET /status/* APIs for Liveness and Readiness Probes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: hfuss <haydenfuss@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 23:59:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Lower default catchup page size
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
        Created At 2022-09-02 00:22:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    Add contract address to filter for catchup
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
        Created At 2022-08-31 19:01:04 +0000 UTC
    </div>
</div>

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

