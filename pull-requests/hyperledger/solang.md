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
                PR <a href="https://github.com/hyperledger/solang/pull/1609" class=".btn">#1609</a>
            </td>
            <td>
                <b>
                    Represent type(f) correctly in the ast
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This makes the ast correct, and also the following code is now parsed correctly:
    
            function foo() {
                    type(int);
            }

 `type(enum-type).min` or `type(enum).min` is now supported. 

This fixes all the issues wrt `type(T)`  in the solc tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 11:48:59 +0000 UTC
    </div>
</div>

