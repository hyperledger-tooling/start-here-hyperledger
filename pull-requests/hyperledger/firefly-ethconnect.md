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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/184" class=".btn">#184</a>
            </td>
            <td>
                <b>
                    Fix post-merge build issue related to error codes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See failure here https://github.com/hyperledger/firefly-ethconnect/runs/4301810830?check_suite_focus=true

Combination of #178 post-merge with #177

```
# github.com/hyperledger/firefly-ethconnect/internal/contractgateway
internal/contractgateway/smartcontractgw.go:529:31: undefined: "github.com/hyperledger/firefly-ethconnect/internal/errors".New
make: *** [Makefile:43: deps] Error 2
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 16:56:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    Do not close a.eventStream, rather handle closed batch dispatcher
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for https://github.com/hyperledger/firefly-ethconnect/issues/182
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 05:44:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/181" class=".btn">#181</a>
            </td>
            <td>
                <b>
                    Reduce default fetch below 1MB in the case of a small circuit breaker upper bound
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After considering  in https://github.com/hyperledger/firefly-ethconnect/pull/175#pullrequestreview-813026469a bit of detail, I came to the conclusion this is a step forwards. Given that:
- Sarama only allows querying the HWM that has most recently been obtained via a fetch
- Configuring the producer to actually consume every message, in order to continually fetch, would be very inefficient 

This isn't perfect, as it still requires the consumer to be actively consuming for the circuit breaker to function.
However, in practice I believe it will protect from overflowing the buffer in the common case as even if the chain were stalled, batches of messages will be being consumed and returned with a timeout error periodically.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 02:31:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/180" class=".btn">#180</a>
            </td>
            <td>
                <b>
                    Fix for intermittent failure #179
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix for #179 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 01:17:00 +0000 UTC
    </div>
</div>

