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
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    Add deploy contract unit tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Refactors the code a little bit for sharing common logic, and to split the implementation/test files
- Adds unit tests for `DeployContractPrepare` FFCAPI implementation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 15:32:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/5" class=".btn">#5</a>
            </td>
            <td>
                <b>
                    When new listener joins avoid delivering events before HWM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When a new listener joins an existing event stream, or catches up to the head group, the filter will be re-established and might re-deliver old events.

For existing listeners, these are innocuous, as they will be de-dup'd by FFTM in the checkpoint (although they're inefficient). 

However, for the new listener joining they could be behind the `fromBlock` specified when the listener was created. Which means you might get events in the past that you would not expect.

There is a "high water mark" tracked on each listener, and move forwards. This is set to the `fromBlock` when a new listener joins. So this PR just enhances the existing post-filter code to discard events that are behind this HWM.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 01:48:29 +0000 UTC
    </div>
</div>

