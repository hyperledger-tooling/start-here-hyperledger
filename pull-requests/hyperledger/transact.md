---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/169" class=".btn">#169</a>
            </td>
            <td>
                <b>
                    Replace checked_sub with saturating_sub
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When I originally wrote this I wanted to use saturating_sub because it
mapped nicely to the requirements but it was one version of Rust off.

Its now stable.

The code removed was copied from the saturating_sub pull request to the
std library so for now there is no real change at all. Going forward relying
on the std lib implementations is preferable to just using unpatched
code snippets copied from pull requests.

Signed-off-by: Caleb Hill <hill@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 13:42:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    Fix struct and module doc for Sqlite backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes the rust doc for the Sqlite backend as well as the migrations module.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 21:39:32 +0000 UTC
    </div>
</div>

