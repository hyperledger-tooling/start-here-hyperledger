---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/200" class=".btn">#200</a>
            </td>
            <td>
                <b>
                    Don't store highestNonce=0 if eth_getTransationCount fails (and solc 8 support)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This snippet below shows that if we get an error on `eth_getTransactionCount`, we seem to go on and perform later processing as if the nonce is zero.

Reviewing the code I found this is because of this is not backed out on error:
https://github.com/hyperledger/firefly-ethconnect/blob/f67b8400a5458e8f73870f75eee067b77cce199f/internal/tx/txnprocessor.go#L260

And in the case EthConnect is fully managing nonces (for example for high concurrency parallel submission), when we come back round for the next time round rather than calling `eth_getTranscationAccount` again,  we will read the `highestNonce` as `0`:
https://github.com/hyperledger/firefly-ethconnect/blob/f67b8400a5458e8f73870f75eee067b77cce199f/internal/tx/txnprocessor.go#L265-L271

My proposed fix, is to defer assignment back to the map until the success return path of the function.

Made two other unrelated changes:
1) Support for compiling EthConnect with `solc` 8 in your path (previously only worked up to `solc` 7)
   - This involved removing the type checking for `byte[]` which is no longer applicable
2) Performing explicit returns in the error paths of `addInflightWrapper` for readability

```
[2022-02-16T12:29:50.935Z]  INFO Received reply message. requestId='0257b3e8-3754-4ec9-70b0-58cf8d200001' reqOffset='' type='Error': eth_getTransactionCount returned: Post "http://localhost:8545": dial tcp 127.0.0.1:8545: connect: connection refused
[2022-02-16T12:29:50.935Z]  INFO 0257b3e8-3754-4ec9-70b0-58cf8d200001: Inserted receipt into receipt store
[2022-02-16T12:29:50.935Z]  INFO Received reply message. requestId='54b6f18a-5c7d-474f-4ac9-cd208403e88a' reqOffset='' type='Error': Call failed: Post "http://10.10.80.27:8545": dial tcp 10.10.80.27:8545: connect: connection refused
[2022-02-16T12:29:50.935Z]  INFO 54b6f18a-5c7d-474f-4ac9-cd208403e88a: Inserted receipt into receipt store
[2022-02-16T12:29:50.935Z]  INFO Received reply message. requestId='6346500f-0308-428d-5a56-10f0a9b50cce' reqOffset='' type='Error': eth_getTransactionCount returned: Post "http://localhost:8545": dial tcp 127.0.0.1:8545: connect: connection refused
[2022-02-16T12:29:50.935Z]  INFO 6346500f-0308-428d-5a56-10f0a9b50cce: Inserted receipt into receipt store
[2022-02-16T12:29:50.935Z]  INFO Received reply message. requestId='ceff65fd-0517-4d5e-410f-c393afe54dfe' reqOffset='' type='Error': Call failed: Post "http://10.10.80.27:8545": dial tcp 10.10.80.27:8545: connect: connection refused
[2022-02-16T12:29:50.935Z]  INFO ceff65fd-0517-4d5e-410f-c393afe54dfe: Inserted receipt into receipt store
[2022-02-16T12:29:50.935Z]  INFO Received reply message. requestId='17e31eae-90bf-4a84-4604-fe87478f0634' reqOffset='' type='Error': eth_getTransactionCount returned: Post "http://localhost:8545": dial tcp 127.0.0.1:8545: connect: connection refused
[2022-02-16T12:29:50.936Z]  INFO 17e31eae-90bf-4a84-4604-fe87478f0634: Inserted receipt into receipt store
[2022-02-16T12:29:50.950Z]  INFO Using cached RPC connection for signing
[2022-02-16T12:29:50.950Z]  INFO In-flight 11361389 added. nonce=2 addr=0xd9db2b11609fdbff838c15b2bcb00dfc03fb6f31 before=1 (node=false)
[2022-02-16T12:29:51.391Z]  WARN TX: Failed to send: nonce too low [0.46s]
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 19:50:47 +0000 UTC
    </div>
</div>

