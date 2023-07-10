---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Avoid double-locking the read-lock calling GetTransactionByIDWithStatus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #95 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-09 17:16:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    Fix confirmations incremental dispatch 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In PR chain with #93 
Also contains commit from #96 

I found that we were re-dispatching the whole set of confirmations each time, in the incremental case where `NewFork: false`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-08 22:50:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    Migration command - leveldb2postgres
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Command line tool helper to perform a LevelDB to PostgreSQL migration.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-07 19:45:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    Provide a way for policy engines to pass additional state to callbacks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Provides an alternative approach the 2nd item in #91 , allowing any policy engine implementation to pass a closure in with additional variables it's safe for that implementation to pass through. For example, a transaction-specific context object.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 20:29:42 +0000 UTC
    </div>
</div>

