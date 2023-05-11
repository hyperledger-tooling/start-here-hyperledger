---
layout: default
title: sawtooth-sdk-rust
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sdk-rust
---

# sawtooth-sdk-rust <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sdk-rust){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-rust/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    fix: Do not panic on channel send failures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The expect() calls here are problematic for async clients, as tasks may be cancelled before the reply channel can be serviced. This can result in spurious errors.

* Use .map_err().ok() rather than expect, so message thread can not panic
* Lower logging to warm
* Log socket errors
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-04 17:48:05 +0000 UTC
    </div>
</div>

