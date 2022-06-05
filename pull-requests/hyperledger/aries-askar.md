---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/52" class=".btn">#52</a>
            </td>
            <td>
                <b>
                    feat: auto commit txn on aexit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an attempt to visualize what #51 would look like. I think it's this simple?

As implemented, instead of an effective "rollback by default", it will rollback if the transaction exits with an exception but otherwise commit by default. The user may still choose to manually call `rollback` before the context is exited.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-05 02:20:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/50" class=".btn">#50</a>
            </td>
            <td>
                <b>
                    Use lock_arc instead of try_lock_arc when borrowing store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #48 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 20:02:09 +0000 UTC
    </div>
</div>

