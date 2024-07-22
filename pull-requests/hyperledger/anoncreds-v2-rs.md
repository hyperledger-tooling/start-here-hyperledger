---
layout: default
title: anoncreds-v2-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-v2-rs
---

# anoncreds-v2-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-v2-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-v2-rs/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    fix formatting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Harold Carr <harold.carr@oracle.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 18:58:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-v2-rs/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    fix out of range panic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Harold Carr <harold.carr@oracle.com>

This adds a test case that expects `InvalidPresentationData` when someone tries to create a range proof with a value that is outside the required range.

Without the fix, it panics:

`thread 'out_of_range_panic' panicked at 'attempt to add with overflow', src/presentation/range.rs:147:38`

This PR adds a check for out of range in `presentation/range.rs` in `RangeBuilder.commit`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 18:27:37 +0000 UTC
    </div>
</div>

