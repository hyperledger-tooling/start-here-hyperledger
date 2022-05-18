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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/218" class=".btn">#218</a>
            </td>
            <td>
                <b>
                    Updates for parallel processing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Three related changes from analysis of some performance tests:

1. The `sendConcurrency` setting is not currently providing the full concurrency support it was intended to. This is because the `concurrencySlots` channel was being allocated in the constructor of the `TxnProcessor` which is before `SetConf` is called. So we need to allocated it in `Init()`. This results in us using pipelining between the `Send` and in-flight nonce allocation, but not performing multiple `Send` calls in parallel. 

2. In the case that a `Send` fails due to an intermittent error, such as a timeout, this is problem for end-users because they do not know if the transaction was submitted or not. However, in cases where EthConnect is in control of the `nonce` it is safe for EthConnect to retry. So this PR introduces an option for retries, and enables these by default (with a small number - 5) to deal with glitches without pushing those errors all the way back to the requester.

3. Currently the addressbook lookup is performed on the single-threaded processing, before we dispatch a concurrent worker to the `inflight` action. As there is a JSON/RPC healthcheck call that is part of this (`net_version`) this is inefficient. So this PR moves it to the concurrent worker, after `inflight` is generated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 15:47:23 +0000 UTC
    </div>
</div>

