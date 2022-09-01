---
layout: default
title: firefly-signer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-signer
---

# firefly-signer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-signer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    Update info logging to include method and time
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly-evmconnect/issues/26

So we have logs like this if only INFO logging is enabled:
```
RPC[2->000012346] <-- eth_getTransactionByHash [200] OK (1.43ms)
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 02:09:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Add underlying error to FF22012
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 15:08:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    Reconcile how we log RPC calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since we merged the RCP client code between EVMConnect and FireFly Signer, we've ended up with a little bit of confusion between the log lines in how we log the RPC request ID.

This PR tries to reconcile it. For EVMConnect where we don't supply an ID, it should look like this:

```log
time="2022-08-29T15:14:23-04:00" level=info msg="RPC[000012346] <-- [200] OK"
```

For FireFly Signer running as a signer, where it also has a front-end ID, it should look like this:

```
time="2022-08-29T15:20:00-04:00" level=info msg="RPC[2->000012346] <-- [200] OK"
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 19:20:22 +0000 UTC
    </div>
</div>

