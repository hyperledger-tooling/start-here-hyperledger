---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1423" class=".btn">#1423</a>
            </td>
            <td>
                <b>
                    Backport 0-3: Use `find` instead of `find_map`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `find` Iterator method takes a closure, which returns a boolean, and
the method then returns the first object that evaluates to true as an
Option, otherwise it returns None. Previously, we were doing this
specification manually in the `find_map` method.

This issue was caught by clippy, for more information on this lint,
see: https://rust-lang.github.io/rust-clippy/master/index.html#unnecessary_find_map

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 17:17:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1422" class=".btn">#1422</a>
            </td>
            <td>
                <b>
                    Use `find` instead of `find_map`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Backport-0-3</span><span class="chip">main</span>
            </td>
            <td>
                The `find` Iterator method takes a closure, which returns a boolean, and
the method then returns the first object that evaluates to true as an
Option, otherwise it returns None. Previously, we were doing this
specification manually in the `find_map` method.

This issue was caught by clippy, for more information on this lint,
see: https://rust-lang.github.io/rust-clippy/master/index.html#unnecessary_find_map

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 16:22:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1421" class=".btn">#1421</a>
            </td>
            <td>
                <b>
                    Add DLT event monitor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                Signed-off-by: Lee Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 20:18:07 +0000 UTC
    </div>
</div>

