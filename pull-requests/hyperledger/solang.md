---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1554" class=".btn">#1554</a>
            </td>
            <td>
                <b>
                    vscode: Use same solang for language server as for compilation on command line
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We've had complaints that the extension gives different errors and warnings than solang on the command line. Use solang from the path and only download solang if it can not be found.

Fixes https://github.com/hyperledger/solang/issues/1444
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 18:48:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1553" class=".btn">#1553</a>
            </td>
            <td>
                <b>
                    Bugfix: Accessing storage struct members is always a storage read
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
        Created At 2023-09-28 08:31:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1552" class=".btn">#1552</a>
            </td>
            <td>
                <b>
                    Bugfix: Variables declared in return param can have a storage location
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Variables declared as return parameters can have a storage location too.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 07:57:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1551" class=".btn">#1551</a>
            </td>
            <td>
                <b>
                    Purge the compiler of `codegen::Expression::List`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The expression was unused.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-22 20:59:02 +0000 UTC
    </div>
</div>

