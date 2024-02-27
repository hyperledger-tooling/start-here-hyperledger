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
                PR <a href="https://github.com/hyperledger/solang/pull/1625" class=".btn">#1625</a>
            </td>
            <td>
                <b>
                    MSRV 1.74 (fixes CI)
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
        Created At 2024-02-27 17:40:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1624" class=".btn">#1624</a>
            </td>
            <td>
                <b>
                    Bugfix: Do not mangle overridden non-overloaded virtual function names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1623 

The basic idea of the algorithm checking whether a function name is eligible for mangling or not is to mangle the name if that function is publicly callable but the functions name appears multiple time in the contract. But this doesn't account for virtual functions also appearing more than one time in the same contract if they are overridden. With this PR, we bail early if the function we are checking overrides, marking only the single one non-overriding implementation as eligible for mangling. Consequently, functions which override but do not overload are no longer unnecessarily mangled.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 17:22:35 +0000 UTC
    </div>
</div>

