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
                PR <a href="https://github.com/hyperledger/grid/pull/733" class=".btn">#733</a>
            </td>
            <td>
                <b>
                    Update CLI PO create to include not-draft option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Man page specifies that there would be both a draft - which is by
default, and a not-draft flag. Updated this implementation to match the
man-page, because draft is a flag and is set to true by default, there
would be no way of setting it to false. Also draft and not-draft is
the convention used for other components. This method is not yet
implemented so it should have no impact on the application.

Signed-off-by: Kevin Johnson <kevin_johnson@cargill.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 12:38:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/732" class=".btn">#732</a>
            </td>
            <td>
                <b>
                    Move `clear_database` fns to new `testing` module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This moves the `clear_database` functions for clearing the postgres and
sqlite databases to a new testing module. These are guarded behind new
features `test-postgres` and `test-sqlite` respectively. This does not
change any functionality.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 21:14:34 +0000 UTC
    </div>
</div>

