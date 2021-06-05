---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/155" class=".btn">#155</a>
            </td>
            <td>
                <b>
                    Human readable rates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a follow up on using floats for rate specifications. Makes it a little less mathy and a little more human
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 16:29:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/154" class=".btn">#154</a>
            </td>
            <td>
                <b>
                    Fix 0-3 merge builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The authorized builders check is triggered erroneously and fails
because merge builds do not have a CHANGE_AUTHOR.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 15:15:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/153" class=".btn">#153</a>
            </td>
            <td>
                <b>
                    Add patch notes for 0.3.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Banks <rbanks@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 16:16:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Generic Merkle State Tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the merkle state tests to use the state traits in all tests that don't involve pruning checks.  This will enable validating the SQL-backed implementation against the same tests.

Additionally, 

- Fixes a bug with error output of the trait implementations in the key-value implementation
- replaces panics with resume_unwind in the test wrappers
- Adds a `key()` accessor to `StateChange`, for convenience
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 14:35:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/151" class=".btn">#151</a>
            </td>
            <td>
                <b>
                    Backport - Update semver dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update sever from 0.9 to 1.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 15:20:38 +0000 UTC
    </div>
</div>

