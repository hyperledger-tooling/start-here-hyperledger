---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/306" class=".btn">#306</a>
            </td>
            <td>
                <b>
                    use time.NewTimer instead of time.After
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using time.After enqueues an entry in Go's runtime scheduler and doesn't garbage collect it even if the function the timer was fired from terminates.
As a result, there can be a temporary high memory pressure and it degrades performance.

Replaced all places where time.After was used except in places where we use it for timing periodical processes (hence, in those places, time.After can only fire when the previous one finishes).

Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 14:16:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/305" class=".btn">#305</a>
            </td>
            <td>
                <b>
                    Expose idemix identity cache size in config
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
        Created At 2022-07-21 13:59:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    Optimize Idemix pre-provision cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit:

- Replaces time.After() with time.NewTimer()
- Only provisions the background workers if needed
- Provisions runtime.NumCPU() background workers
  to reduce waiting time in case of high bursts

Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 13:32:41 +0000 UTC
    </div>
</div>

