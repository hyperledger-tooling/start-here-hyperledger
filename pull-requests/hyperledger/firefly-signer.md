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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    omitempty Value and Gas for ethsigner.Transaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://ethereum.org/en/developers/docs/apis/json-rpc/#eth_sendtransaction with `value` being an optional field, this will prevent it from being serialized and passed through in JSONRPC requests when set to `nil`.

We encountered https://github.com/hyperledger/firefly-evmconnect passing `nil` `value` down to our managed signer which passed it along to the chain and received an RPC error as a result:
```
[2022-08-24T21:06:20.566Z]  INFO id=29337 method=eth_sendTransaction params=[map[data:0x48ce1dcce6ba6ce9bbd44a5a955d32e79d5f6d9d38559556a2364b60933c0ab216077c8a1cbf6f208b2b0afa8bf5b242388dca09a30d32af1b7adcc604d53f4b05d2b50c000000000000000000000000000000000000000000000000000000000000008000000000000000000000000000000000000000000000000000000000000000e0000000000000000000000000000000000000000000000000000000000000002e516d5448535947415a5073424a735548746957537366344777386a364e4a62514172547274794364714d6e79736b0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001471a8843524eddfda67a8769c3ac0ebf5fef87536989ae928b88fcd4fbed6866 from:0xad6d779ca7603abc0115ec7de57c89828993be19 gas:0xbb8a gasPrice:0x0 nonce:0x6 to:0xe21906c40fef96d4cee3c43bf8da724ac8783510 value:<nil>]]
...
[2022-08-24T21:06:20.566Z]  INFO Sending JSON/RPC error: Code=-32600 ID=29337 Message=''value' could not be converted to an integer: unexpected type <nil> for BigInt'
```

confirmed this works as a fix as part of testing https://github.com/hyperledger/firefly-evmconnect/pull/19.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 03:29:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    Move RPC Client code to shared package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We had some duplicated code between `firefly-evmconnect` and `firefly-signer`. This PR moves the updated RPC error handling and logging from evmconnect into signer, and exposes it as a shared package. I'm about to open a subsequent PR for evmconnect that uses this package so there is one place this code exists now instead of two.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 19:36:39 +0000 UTC
    </div>
</div>

