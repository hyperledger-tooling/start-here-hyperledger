---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3036" class=".btn">#3036</a>
            </td>
            <td>
                <b>
                    docs(build): change NodeJS version in BUILD.md to v18.18.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fix node version in BUILD.md what caused type error in corepack
and prevented yarn from installing packages correctly.
Error message when using node 16: Type Error: URL.canParse is not a function

Signed-off-by: Tomasz Awramski <tomasz.awramski@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 14:23:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3035" class=".btn">#3035</a>
            </td>
            <td>
                <b>
                    test(cbdc-example): removed dependency on chai and update tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Chai was removed as dependency of the cbdc-backend package
* A test scenario was removed in the 'bridge-back' feature due to having duplicated logic with another one in the same file
* Some tests were failing due to timeouts, so we added an explicit and generous timeout limit for each step

closes #3034
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-28 17:07:46 +0000 UTC
    </div>
</div>

