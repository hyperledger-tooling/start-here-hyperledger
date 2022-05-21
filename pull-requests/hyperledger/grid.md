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
                PR <a href="https://github.com/hyperledger/grid/pull/1425" class=".btn">#1425</a>
            </td>
            <td>
                <b>
                    Update Grid to use `actix_web` 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">main</span>
            </td>
            <td>
                This updates grid to use `actix_web` v4. Both v3 and 4 cannot be supported in Grid due to conflicting re-exports of tokio structs/traits from the libraries. Therefore, all rest api code and tests in the Grid SDK, Griddle, and the Grid Daemon is updated to use actix_web 4.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 19:16:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1424" class=".btn">#1424</a>
            </td>
            <td>
                <b>
                    Add submitter and observer traits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                Adds the public traits for the submitter and submitter observer. These will be used in future implementations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 16:27:47 +0000 UTC
    </div>
</div>

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

