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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/67" class=".btn">#67</a>
            </td>
            <td>
                <b>
                    Update build and test scripts
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
        Created At 2023-11-14 06:08:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/66" class=".btn">#66</a>
            </td>
            <td>
                <b>
                    Change WebSocket dependency to a stable one
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Revision dependency only works in dev mode. We must use a tag for dependencies.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-13 06:13:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/65" class=".btn">#65</a>
            </td>
            <td>
                <b>
                    Replace Indy SDK and convert to a Swift package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Close #29 

This is a bulk update with the following changes:
- Replace Indy SDK
- Convert to a Swift package
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-13 05:39:37 +0000 UTC
    </div>
</div>

