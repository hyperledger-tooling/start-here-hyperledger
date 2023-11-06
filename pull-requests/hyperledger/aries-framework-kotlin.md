---
layout: default
title: aries-framework-kotlin
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-kotlin
---

# aries-framework-kotlin <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-kotlin){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-kotlin/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Fix type casting error when using 'as' keyword
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. I changed the `var agent` property to use `lateinit` so it can be used without `!!`.

2. I ran into the following errors, and fixed this type casting by calling the `toInt()` and `toLong()` methods.

```
java.lang.ClassCastException: java.lang.Integer cannot be cast to java.lang.Long
    at org.hyperledger.ariesframework.ledger.LedgerService.getRevocationRegistryDelta(LedgerService.kt:122)
    at org.hyperledger.ariesframework.proofs.RevocationService.getRevocationStatus(RevocationService.kt:67)
    at org.hyperledger.ariesframework.proofs.ProofService.getRevocationStatusForRequestedItem(ProofService.kt:344)
    at org.hyperledger.ariesframework.proofs.ProofService$getRequestedCredentialsForProofRequest$lambda$2$$inlined$concurrentMap$1.invokeSuspend(ConcurrentTransform.kt:37)
    at kotlin.coroutines.jvm.internal.BaseContinuationImpl.resumeWith(ContinuationImpl.kt:33)
    at kotlinx.coroutines.DispatchedTask.run(DispatchedTask.kt:106)
    at kotlinx.coroutines.scheduling.CoroutineScheduler.runSafely(CoroutineScheduler.kt:584)
    at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.executeTask(CoroutineScheduler.kt:793)
    at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.kt:697)
    at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.kt:684)
```

```
java.lang.ClassCastException: java.lang.Integer cannot be cast to java.lang.Long
    at org.hyperledger.ariesframework.proofs.RevocationService$createRevocationState$$inlined$concurrentForEach$1.invokeSuspend(ConcurrentTransform.kt:60)
    at kotlin.coroutines.jvm.internal.BaseContinuationImpl.resumeWith(ContinuationImpl.kt:33)
    at kotlinx.coroutines.DispatchedTask.run(DispatchedTask.kt:106)
    at kotlinx.coroutines.scheduling.CoroutineScheduler.runSafely(CoroutineScheduler.kt:584)
    at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.executeTask(CoroutineScheduler.kt:793)
    at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.runWorker(CoroutineScheduler.kt:697)
    at kotlinx.coroutines.scheduling.CoroutineScheduler$Worker.run(CoroutineScheduler.kt:684)
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 07:57:08 +0000 UTC
    </div>
</div>

