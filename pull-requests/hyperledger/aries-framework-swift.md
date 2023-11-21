---
layout: default
title: aries-framework-swift
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-swift
---

# aries-framework-swift <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-swift){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/72" class=".btn">#72</a>
            </td>
            <td>
                <b>
                    Use macos-13 runner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Try to fix #70
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-16 04:58:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/71" class=".btn">#71</a>
            </td>
            <td>
                <b>
                    Use AsyncSemaphore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use AsyncSemaphore instead of NSLock.
Previous usage was not safe and this change removes build warning.

References:
- https://forums.swift.org/t/what-does-use-async-safe-scoped-locking-instead-even-mean/61029/8
- https://github.com/groue/Semaphore
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-14 11:41:17 +0000 UTC
    </div>
</div>

