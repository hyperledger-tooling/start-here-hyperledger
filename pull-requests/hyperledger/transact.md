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
                PR <a href="https://github.com/hyperledger/transact/pull/129" class=".btn">#129</a>
            </td>
            <td>
                <b>
                    Fix manual implementation of Option::map lint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes a lint introduced in the 1.52.0 release of Rust
flagging items like

    match Some(0) {
        Some(x) => Some(x + 1),
        None => None,
    };

Use instead:

    Some(0).map(|x| x + 1);

In some cases this requires an `as &(dyn Error + 'static)`

See for
    https://rust-lang.github.io/rust-clippy/master/index.html#manual_map
for details

Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 15:46:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/128" class=".btn">#128</a>
            </td>
            <td>
                <b>
                    Update justfile to build additional feature combinations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are two features enabled during testing which were not previously
built in the justfile. One is sawtooth compat and the other is
redis-related tests. This modification builds both of these to make it
easier to detect compilation errors which impact those features.

Signed-off-by: Shawn T. Amundson <amundson@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 18:44:42 +0000 UTC
    </div>
</div>

