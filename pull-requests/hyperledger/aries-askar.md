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
                PR <a href="https://github.com/hyperledger/aries-askar/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    fix(js): promise handle error and rn updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some additional updates after #209.

It addresses two things:
- also handle error code mismatch in the promise callback
- update the RN implementation to handle the errors in the same way as we updated to in the node js wrapper. @berendsliedrecht you mentioned it was already implemented correctly in RN, were you talking about the unnessary error calling? Because the code matching logic was not present in the RN wrapper.

I've changed the mismatch behaviour handling to now throw an error with the original errorCode, and a custom message "Error has already been overwritten, unable to provide error message". That way it won't break the calling implementation, as long as they use errorCodes to  handle errors. I've looked and it seems we're not using error message from Askar anymore to do error handling, so this should fix the problem, except for not always having the correct error message in the logs.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-21 08:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/210" class=".btn">#210</a>
            </td>
            <td>
                <b>
                    Refactor FFI error handling for better reliability
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
        Created At 2023-12-19 19:38:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/209" class=".btn">#209</a>
            </td>
            <td>
                <b>
                    fix(nodejs): only call get_current_error when an error occurred
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Reduce additional calls to `get_current_error`
- Added tests for resolving errors for sync and async calls
    - async calls include error handling inside the callback and outside

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 16:05:09 +0000 UTC
    </div>
</div>

