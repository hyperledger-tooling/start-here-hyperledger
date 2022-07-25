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
                PR <a href="https://github.com/hyperledger/cello/pull/472" class=".btn">#472</a>
            </td>
            <td>
                <b>
                    Enable Github CI for Code Check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Create yml file to run the code check CI.
- Fix version of eslint-plugin-import to avoid a known bug in it.
- Replace `make docker` in Makefile with new commands.

Signed-off-by: Xichen Pan <xichen.pan@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 01:13:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/470" class=".btn">#470</a>
            </td>
            <td>
                <b>
                    Fix code format issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix the code format issues found by flake8 and eslint during `make check`.

Signed-off-by: Xichen Pan [xichen.pan@gmail.com](mailto:xichen.pan@gmail.com)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 04:30:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/469" class=".btn">#469</a>
            </td>
            <td>
                <b>
                    fix(security):Command Injection and Path Traversal Bugs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Fix 1 - Path Traversal

Unsanitized input from the HTTP request body [request.data] flows into os.walk, where it is used as a path. This may result in a Path Traversal vulnerability and allow an attacker to read arbitrary files.

## Fix 2 - Command Injection

Unsanitized input from the HTTP request body [request.data] flows into os.system, where it is used as a path. This may result in a Path Traversal vulnerability and allow an attacker to read arbitrary files.


Signed-off-by: Bhaskar <ram@hacker.ind.in>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 08:11:22 +0000 UTC
    </div>
</div>

