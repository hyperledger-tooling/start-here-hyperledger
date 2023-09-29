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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1549" class=".btn">#1549</a>
            </td>
            <td>
                <b>
                    Support `address.code` in sema
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
        Created At 2023-09-22 15:25:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1548" class=".btn">#1548</a>
            </td>
            <td>
                <b>
                    Add code coverage bot 🤖
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Coverage reports will be stored [here](https://app.codecov.io/gh/hyperledger/solang).

According to Codecov's documentation,
> Once merged to the default branch, subsequent pull requests will have checks and report comment.

This is an example of how comments look like: https://github.com/solana-labs/solana/pull/33363#issuecomment-1730528544
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-22 14:53:16 +0000 UTC
    </div>
</div>

