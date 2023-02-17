---
layout: default
title: fabric-admin-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-admin-sdk
---

# fabric-admin-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-admin-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    Fix staticcheck checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                staticcheck was only being run against the root directory, which contains no Go files. Change to run recurseively so code is actually checked.

For now, disable checks for missing package documentation.

Fix staticcheck failures and remove use of unnecessary github.com/pkg/errors package.

Disable fail-fast for golang test matrix so all test results can be viewed, even if one fails.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 18:21:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    Refactor query committed functions to use gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Now query committed functions use the evaluate method of the gateway service, as suggested by @bestbeforetoday in #89 
- Unit tests were re-written
- No changes were necessary to E2E test

Signed-off-by: Samuel Venzi <samuel.venzi@me.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 23:24:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-admin-sdk/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    add validation phase to same with fabric CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add validation phase to same with fabric CLI

Signed-off-by: Sam Yuan <yy19902439@126.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-11 11:42:04 +0000 UTC
    </div>
</div>

