---
layout: default
title: besu-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-native
---

# besu-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    Preparing for next release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Lucas Saldanha <lucascrsaldanha@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 04:28:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    Release 0.4.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Lucas Saldanha <lucascrsaldanha@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 03:53:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/52" class=".btn">#52</a>
            </td>
            <td>
                <b>
                    Padding of the R and S components in case they are smaller than 31 bytes for SECP256r1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                _Note from @NicolasMassart (Consensys Customer Support):
This PR if from one of the Consensys customers directly. I removed the internal reference to our ticketing system as it's not useful to HL community as they don't have access. The PR is well referenced in the ticket on our side._

## Description of the issue

Sometimes the signature components (in that case it was R) are 30-bytes long and both the keys and the signatures are still valid.

The values added in the unit test are taken from one of the actual errors shown in the error logs:

```
2022-01-19 17:39:09.672+00:00 | EthScheduler-Workers-1 | INFO  | PersistBlockTask | Imported #591,672 / 22 tx / 0 om / 784,208 (0.0%) gas / (0x14eb9590af60f2e86d4a617bb34e8de4255b35819cfbb8a1a87dc0cbbc021b21) in 0.065s. Peers: 4
2022-01-19 17:39:10.032+00:00 | vert.x-worker-thread-3 | ERROR | JsonRpcHttpService | Error processing JSON-RPC requestBody
java.lang.IllegalStateException: Cannot recover public key from signature for MessageCall{type=FRONTIER, nonce=354537, gasPrice=0x0, gasLimit=900000, to=0x4bdf5ccc513a0f4c9e70f8e22dc572c6a3ce93f3, value=0x0000000000000000000000000000000000000000000000000000000000000000, sig=Signature{r=607232317131644998607993399928086035368869502933999419429470745918733484, s=909326537358980219114547956988636184748037502936154044628658501523731230682, recId=1}, payload=0x2b96ec34000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000000ce080112a3010a14d4e799019fb8850f5532baafb57302ae7ad4daad1220c57f3ba81cb7fd341e18dcbbf29ee2e1de8fa0253099304f7fd92088b895f5d51a473045022100ef44c089e8e099cabea07b002985876c543194b0bc00415fef8cee5b8f6e8e6b02205580d481f79fb1f6ee2b541738b79481d89c159c3c39cd9b438d3e52c29065122220088116856e9d1d554d9f0d51de6405b25d1f5eabca81f7a3781145830f975a4f2a2431643265633838612d626431372d343565342d383535622d653962656536363565666331000000000000000000000000000000000000}
	at org.hyperledger.besu.ethereum.core.Transaction.lambda$getSender$3(Transaction.java:517)
	at java.base/java.util.Optional.orElseThrow(Optional.java:408)
	at org.hyperledger.besu.ethereum.core.Transaction.getSender(Transaction.java:515)
	at org.hyperledger.besu.ethereum.mainnet.MainnetTransactionValidator.validateTransactionSignature(MainnetTransactionValidator.java:257)
	at org.hyperledger.besu.ethereum.mainnet.MainnetTransactionValidator.validate(MainnetTransactionValidator.java:111)
	at org.hyperledger.besu.ethereum.eth.transactions.TransactionPool.validateTransaction(TransactionPool.java:240)
	at org.hyperledger.besu.ethereum.eth.transactions.TransactionPool.addLocalTransaction(TransactionPool.java:135)
	at org.hyperledger.besu.ethereum.api.jsonrpc.internal.methods.EthSendRawTransaction.response(EthSendRawTransaction.java:79)
	at org.hyperledger.besu.ethereum.api.jsonrpc.JsonRpcHttpService.process(JsonRpcHttpService.java:748)
	at org.hyperledger.besu.ethereum.api.jsonrpc.JsonRpcHttpService.lambda$handleJsonSingleRequest$14(JsonRpcHttpService.java:608)
	at io.vertx.core.impl.ContextImpl.lambda$null$0(ContextImpl.java:159)
	at io.vertx.core.impl.AbstractContext.dispatch(AbstractContext.java:100)
	at io.vertx.core.impl.ContextImpl.lambda$executeBlocking$1(ContextImpl.java:157)
	at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1128)
	at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:628)
	at io.netty.util.concurrent.FastThreadLocalRunnable.run(FastThreadLocalRunnable.java:30)
	at java.base/java.lang.Thread.run(Thread.java:829)
2022-01-19 17:39:11.668+00:00 | EthScheduler-Workers-1 | INFO  | PersistBlockTask | Imported #591,673 / 11 tx / 0 om / 392,072 (0.0%) gas / (0xda0059d5397a909d9f7ffd5b178e323da9f3623a36eb0d60843209ff8d8ab894) in 0.036s. Peers: 4
```

There is [another test created in this fork on an upper level for Besu](https://github.com/freemanzMrojo/besu/blob/test-signature-r-padded-r1/crypto/src/test/java/org/hyperledger/besu/crypto/SECP256R1Test.java#L150) checking precisely the same as this test.

## Fix

Add proper padding to signatures

Signed-off by: miguelangel.rojofernandez@mastercard.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 18:05:18 +0000 UTC
    </div>
</div>

