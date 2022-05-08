---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/441" class=".btn">#441</a>
            </td>
            <td>
                <b>
                    [#issue-439] Fix the issue of long debug info in http response body.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [#issue-439] Fix the issue of long debug info in http response body.

Cause of issue:

```python3
# at src/dashboard/src/utils/request.js
Line 48: err(e), status=status.HTTP_409_CONFLICT

```
err(e) contains all the debug information, and should be replaced with a better error message.

Solution:
replace object e with better error messages like 'Email Aleady exists!'.

Additional Features:
I implemented notifications for login and register error message in dashboard.

Signed-off-by: ada2468 <jx2161@nyu.edu>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-07 02:10:24 +0000 UTC
    </div>
</div>

